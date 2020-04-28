directories %w(. app)

##############################################################################
# APP CODE
##############################################################################

# APP HAML
guard :haml, input: 'app/markup', output: 'public'

# APP SASS
guard :sass, input: 'app/style', output: 'public/style'

# APP COFFEE
coffeescript_options = {
  input: 'public/script',
  output: 'public/script',
  patterns: [/app\/script/]
}
guard 'coffeescript', coffeescript_options do
  coffeescript_options[:patterns].each { |pattern| watch(pattern) }
end

# APP ASSETS
guard :copy, from: 'app/images', to: 'public/images'

##############################################################################
# VENDOR CODE
# Third-party library code
##############################################################################

# VENDOR JS
guard :copy, from: 'vendor/script', to: 'public/script'

# VENDOR CSS
guard :copy, from: 'vendor/style', to: 'public/style'

##############################################################################
# LIVE RELOAD
##############################################################################


guard 'livereload' do
  watch(/public\/.+\.(html|js|css)/)
end

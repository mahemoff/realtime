directories %w(. app)

# HAML
guard :haml, input: 'app/markup', output: 'public'

# SASS
guard :sass, input: 'app/style', output: 'public/style'

# COFFEE
coffeescript_options = {
  input: 'public/script',
  output: 'public/script',
  patterns: [/app\/script/]
}
guard 'coffeescript', coffeescript_options do
  coffeescript_options[:patterns].each { |pattern| watch(pattern) }
end

guard 'livereload' do
  watch(/public\/.+\.(html|js|css)/)
end

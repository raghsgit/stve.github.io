ignore /\_site/, /public/

guard 'coffeescript', :input => 'coffee', :output => 'javascripts'

guard 'compass' do
  watch(%r{^sass\/(.*)\.scss})
end

guard 'jekyll' do
  watch('_config.yml')
  watch(%r{^(index|about|archives|404|colophon)\.html})
  watch(%r{^(atom|sitemap)\.xml})
  watch(%r{^_includes\/(.*)})
  watch(%r{^_layouts\/(.*)})
  watch(%r{^_plugins\/(.*)\.rb})
  watch(%r{^_posts\/(.*)\.(markdown|md)})
  watch(%r{^(javascripts|fonts|stylesheets|images)\/.*})
end

guard 'puma', :port => 4000 do
  watch('Gemfile.lock')
  watch('config.ru')
end

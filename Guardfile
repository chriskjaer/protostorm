guard 'haml', 
  :output => 'public', 
  :input => 'src', 
  :notifications => true, 
  :run_at_start => true do
    watch %r{^src/.+(\.haml)}
  end

guard 'sass',
  :input => 'assets/sass',
  :output => 'public/styles',
  :compass => true,
  :compass => {
    :images_dir       => "assets/images",
    :images_path      => File.join(Dir.pwd, "public/images"),
    :http_images_path => "/images",
    :http_images_dir  => "/images",
    :http_fonts_path  => "/styles/fonts",
    :http_fonts_dir   => "/styles/fonts"
  },
  :smart_partials => true,
  :load_paths => ['vendor']

guard 'livereload' do
  watch(%r{public/.+\.(css|js|html)})
end

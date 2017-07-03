require 'html-proofer'

task :default do
  sh "bundle exec jekyll build"
  options = {
    :assume_extension => true,
    :checks_to_ignore => ["ImageCheck"],
    :url_ignore => ["https://linkedin.com/in/krtierney"]
  }
  HTMLProofer.check_directory("./_site", options ).run
end

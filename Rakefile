require 'html-proofer'

task :default do
  sh "bundle exec jekyll build"
  options = { :assume_extension => true }
  HTMLProofer.check_directory("./_site", { :checks_to_ignore => ["ImageCheck"] } ).run
end

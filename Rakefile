require 'html-proofer'
require 'rubocop/rake_task'

task :default do
  sh 'bundle exec jekyll build'
  opts = {
    assume_extension: true,
    checks_to_ignore: ['ImageCheck'],
    url_ignore: ['https://linkedin.com/in/krtierney', 'https://www.happybearsoftware.com']
  }
  HTMLProofer.check_directory('./_site', opts).run
  RuboCop::RakeTask.new(:rubocop) do |t|
    t.options = ['--display-cop-names']
  end
end

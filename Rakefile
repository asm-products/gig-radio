desc "Deploy to S3"
task :deploy do
  # Don't jekyll build yet!
  # system "jekyll build"
  
  # I'm authentcated on S3 for s3cmd. getgigradio.com is the root domain bucked name
  system "s3cmd sync _site/* s3://getgigradio.com --delete-removed -P"
end

task :default => :deploy

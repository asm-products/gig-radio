desc "Deploy to S3"
task :deploy do
  system "jekyll build"
  system "s3cmd sync _site/* s3://gigradio-website --delete-removed -P"
end

task :default => :deploy

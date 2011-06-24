# Adopted from Tate Johnson's Rakefile
# http://github.com/tatey/tatey.com/blob/master/Rakefile

task :default => :server
 
desc 'Build site with jekyll'
task :build do
  jekyll
end
 
desc 'Start server with --auto'
task :server do
  jekyll('--server --auto')
end

desc 'Build and deploy'
task :deploy => :build do
  sh "rsync -rtzh --progress --delete _site/ --exclude '/photo' rouge8_andyfreeland@ssh.phx.nearlyfreespeech.net:/home/public/"
end

def jekyll(opts = '')
  sh 'rm -rf _site'
  sh 'jekyll ' + opts
end

# Adopted from Tate Johnson's Rakefile
# http://github.com/tatey/tatey.com/blob/master/Rakefile

task :default => :server
 
desc 'Build site with ejekyll'
task :build do
  ejekyll
end
 
desc 'Start server with --auto'
task :server do
  ejekyll('--server --auto')
end

desc 'Build and deploy'
task :deploy => :build do
  sh 'rsync -rtzh --progress  _site/ rouge8_andyfreeland@ssh.phx.nearlyfreespeech.net:/home/public/'
end

def ejekyll(opts = '')
  sh 'rm -rf _site'
  sh 'ejekyll ' + opts
end

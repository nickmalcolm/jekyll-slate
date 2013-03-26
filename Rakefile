desc "compile and run the site"
task :run do
  pids = [
    spawn("jekyll --auto --server"), # put `auto: true` in your _config.yml
  ]
 
  trap "INT" do
    Process.kill "INT", *pids
    exit 1
  end
 
  loop do
    sleep 1
  end
end
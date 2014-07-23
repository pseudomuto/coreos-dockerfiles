REPO_OWNER = "pseudomuto".freeze

desc "Build the specified image"
task :build, [:image] do |t, args|
  sh "cd ./#{args.image} && sudo docker build -t=\"#{REPO_OWNER}/#{args.image}\" ."
end

desc "Push the specified image to docker registery"
task :push, [:image] do |t, args|
  sh "sudo docker push #{REPO_OWNER}/#{args.image}"
end

desc "Create a new image"
task :new, [:image] do |t, args|
  sh "cp -R _template/ #{args.image}"
  sh "sed -i 's/\\$\\$NAME\\$\\$/#{args.image}/g' #{args.image}/*"
end

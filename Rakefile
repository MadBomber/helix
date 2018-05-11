desc "Test Helix Examples"
task :test do
  cd "ruby" do
    sh "bundle exec rake"
  end

  examples = ENV["EXAMPLES"] || "duration calculator console geometry membership text_transform turbo_blank json_builder"

  sh "bash ./examples/runner default #{examples}"
end

desc "Install Helix Examples"
task :install do
  cd "ruby" do
    sh "bundle"
  end

  examples = ENV["EXAMPLES"] || "duration calculator console geometry membership text_transform turbo_blank json_builder"

  sh "bash ./examples/runner install #{examples}"
end

task :default => :test

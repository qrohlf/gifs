task :update do
  gifs = Dir['*.gif']
  puts gifs
  File.open("README.md", 'w') do |readme|
    readme << "# @qrohlf's reaction gif stash\n\n"
    gifs.each do |gif|
      readme << "## #{gif}\n\n"
      readme << "![](#{gif})\n\n"
    end
  end
end

task default: :update

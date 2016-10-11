namespace :assets do
  task :precompile do
    puts `bundle exec jekyll build`
  end
end

namespace :deploy do
	task :local do
		puts "Server address: http://127.0.0.1:4000/"
		puts `bundle exec jekyll serve --watch`
	end

	task :prod do
		puts `bundle exec puma -t 8:32 -w 3 -p $PORT`
	end
end

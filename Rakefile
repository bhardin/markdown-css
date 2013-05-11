#!/bin/ruby
require 'rake'
require 'redcarpet'

task :default => [:build] 

desc "Build the html files based on the css files in the directory"
task :build do
  css_file_list = FileList.new('*.css')

	markdown = Redcarpet::Markdown.new(Redcarpet::Render::HTML, :autolink => true, :space_after_headers => true)

	css_file_list.each do | css_file |
		begin
			filename = css_file.split('.')[0] + ".html"
		  html_file = File.open(filename, "w")
		  html_file.write("<html><body>")

		  html_file.write("<head>")
		  html_file.write("<link href='http://fonts.googleapis.com/css?family=Alice|Alfa+Slab+One' rel='stylesheet' type='text/css'>")
		  html_file.write("</head>")
		  
		  css_file_list.each do | css_link |
		  	css = css_link.split('.')[0]
			  html_file.write markdown.render("[#{css} Theme](#{css}.html)")
			end
			
			html_file.write "<link rel='stylesheet' href='#{css_file}'/>"
			html_file.write markdown.render(File.open("sample.md").read)
			html_file.write("</body></html>")
			#html_file.write sample.md
		rescue IOError => e
		  #some error occur, dir not writable etc.
		ensure
		  html_file.close unless html_file == nil
		end
	end
end







resume_name = "michael-ficarra"
task :default => [:pdf,:open]

task :pdf do |task,args|
	sh "pdflatex #{resume_name}.tex"
	sh "rm #{resume_name}.aux #{resume_name}.log"
end

task :clean do |task,args|
	sh "rm -f #{resume_name}.pdf #{resume_name}.ps"
end

task :open do |task,args|
	sh "open #{resume_name}.pdf"
end

task :default => :compile

file :compile => %w{confusingsolvedppcr.jison} do
  sh "jison confusingsolvedppcr.jison confusingsolvedppcr.l -o confusingsolvedppcr.js"
end

task :clean do
  sh "rm -f confusingsolvedppcr.err  confusingsolvedppcr.output confusingsolvedppcr.tab.jison  confusingsolvedppcr.js confusingsolvedppcr.bak"
end

desc "print files"
task :print do
  sh "a2ps --columns=1 -f 8 -R confusingsolvedppcr.jison -o out.ps"
end

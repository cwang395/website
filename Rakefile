GH_PAGES_DIR = "compiled_site"
ORIGIN_REPO = "https://github.com/cwang395/website.git"

desc "Build Jekyll site and copy files"
task :build do
  system "jekyll build"
  if not File.exists? "../#{GH_PAGES_DIR}/"
    system "mkdir ../#{GH_PAGES_DIR}/"
    system "cd ../#{GH_PAGES_DIR}/ && git init . && git remote add origin #{ORIGIN_REPO}"
  end
  system "rm -r ../#{GH_PAGES_DIR}/*" unless Dir['../#{GH_PAGES_DIR}/*'].empty?
  system "cp -r _site/* ../#{GH_PAGES_DIR}/"
end


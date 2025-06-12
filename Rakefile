desc "Bump version in preparation of a release"
task 'vox:version:bump:full', [:version] do |_, args|
  File.write('VERSION', "#{args[:version]}\n")
end

desc 'Mock release preparation task'
task 'release:prepare' do
  sh 'echo "release $(cat VERSION) on $(date)" >> CHANGELOG'
end

NAME = "ImageLoader"
WORKSPACE = "#{NAME}.xcworkspace"

task :test do
  sh "carthage bootstrap --platform iOS"
  sh "xcodebuild clean -workspace #{WORKSPACE} -scheme #{NAME} -sdk iphonesimulator9.2 -destination 'platform=iOS Simulator,name=iPhone 6,OS=9.2' build test | xcpretty -c"
end

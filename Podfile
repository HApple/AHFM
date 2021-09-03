# Uncomment the next line to define a global platform for your project
platform :ios, '11.0'

source 'https://github.com/iOSModularization/AHFMSpecs.git'
source 'https://github.com/CocoaPods/Specs.git'

post_install do |installer|
    installer.pods_project.targets.each do |target|
        target.build_configurations.each do |config|
            config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '11.0'
            config.build_settings['SWIFT_VERSION'] = '5.0'
        end
    end
end


target 'AHFM' do
  # Comment the next line if you're not using Swift and don't want to use dynamic frameworks
  use_frameworks!

	pod 'AHServiceRouter'
	pod 'AHFMMainServices'
	pod 'AHFMMainManager'
    pod 'AHFMMain'

end

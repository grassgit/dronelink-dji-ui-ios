platform :ios, '12.0'
inhibit_all_warnings!
use_frameworks!

target 'DronelinkDJIUI' do
  pod 'DronelinkCore', '~> 1.7.0'
  pod 'DronelinkCoreUI', '~> 1.5.0'
  pod 'DronelinkDJI', '~> 1.8.0'
  pod 'DJI-UXSDK-iOS', '~> 4.13'
  pod 'SwiftyUserDefaults', '~> 5.0.0'
  pod 'SnapKit', '~> 5.0.1'
  pod 'MaterialComponents/Palettes', '~> 115.0.0'
  post_install do |installer|
    installer.pods_project.targets.each do |target|
      target.build_configurations.each do |config|
        config.build_settings['ENABLE_BITCODE'] = 'NO'
      end
    end
  end
end
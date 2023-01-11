platform :ios, '11.0'
use_frameworks!
#屏蔽警告
inhibit_all_warnings!
targetsArray = ['TestUpload']
targetsArray.each do |t|
    target t do
      pod 'IQKeyboardManagerSwift'
    end
end

post_install do |pi|
    pi.pods_project.targets.each do |t|
      t.build_configurations.each do |config|
        config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '11.0'
      end
    end
end

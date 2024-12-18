platform :osx, '10.13'
inhibit_all_warnings!

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      # 指定最开发版本
      config.build_settings['MACOSX_DEPLOYMENT_TARGET'] = '10.13'
    end
  end
end
target 'Seaglass' do
  use_frameworks!
  pod 'OLMKit', :git=> 'https://gitlab.matrix.org/matrix-org/olm.git',:tag => '2.2.2'
  pod 'SwiftMatrixSDK', :git=> 'https://github.com/HeHuiqi/MatrixSDK_0.10.12.git'
  pod 'Down'
  pod 'TSMarkdownParser'
  pod 'Sparkle'
  pod 'LetsMove'
end

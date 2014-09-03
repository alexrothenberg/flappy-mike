# -*- coding: utf-8 -*-
$:.unshift("/Library/RubyMotion/lib")
require 'motion/project/template/ios'

begin
  require 'bundler'
  Bundler.require
rescue LoadError
end

Motion::Project::App.setup do |app|
  # Use `rake config' to see complete project settings.
  app.name = 'Flappy Mike'

  app.codesign_certificate = 'iPhone Distribution: alex rothenberg (WMBATEPB4K)'
  app.identifier           = 'com.alexrothenberg.flappymike'
  app.provisioning_profile = '/Users/alex/Library/MobileDevice/Provisioning Profiles/e56f3e46-9465-4f00-9f5b-19420d40a9d3.mobileprovision'

  # app.testflight.sdk = 'vendor/TestFlightSDK'
  app.testflight.api_token  = ENV['TESTFLIGHT_API_TOKEN']
  app.testflight.team_token = ENV['TESTFLIGHT_TEAM_TOKEN']

  app.frameworks = %w(CoreGraphics AVFoundation UIKit QuartzCore SpriteKit Foundation)

  app.interface_orientations = [:portrait]
  app.icons = %w(app_icon_iphone.png app_icon_iphone@2x.png)

  # app.release do
    # This entitlement is required during development but must not be used for release.
    app.entitlements['get-task-allow'] = false
  # end
end

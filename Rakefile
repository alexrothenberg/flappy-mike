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

  app.frameworks = %w(CoreGraphics AVFoundation UIKit QuartzCore SpriteKit Foundation)

  app.interface_orientations = [:portrait]
  app.icons = %w(app_icon_iphone.png app_icon_iphone@2x.png)
end

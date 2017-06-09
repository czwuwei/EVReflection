source 'https://github.com/CocoaPods/Specs.git'
use_frameworks!
workspace 'EVReflection'

def swift4libraries
    pod 'Alamofire', :git => 'https://github.com/Alamofire/Alamofire.git' , :branch => 'swift4'
end

# Our Libraries (just include everything for the demo)
def alllibraries
  pod 'EVReflection/MoyaRxSwiftXML', :path => "./"
  pod 'EVReflection/MoyaReactiveSwiftXML', :path => "./"
  pod 'EVReflection/Realm', :path => "./"
  pod 'EVReflection/CloudKit', :path => "./"
  pod 'EVReflection/CoreData', :path => "./"
  swift4libraries
end

target 'PerformanceTest' do
  project 'PerformanceTest/PerformanceTest'
  platform :ios, '8.0'
  pod 'EVReflection/Core', :path => "./"
end


target 'UnitTestsiOS' do
    project 'UnitTests/UnitTests'
    platform :ios, '8.0'
    alllibraries
end

target 'UnitTestsOSX' do
    project 'UnitTests/UnitTests'
    platform :osx, '10.11'
    alllibraries
end

target 'UnitTestsTVOS' do
    project 'UnitTests/UnitTests'
    platform :tvos, '9.0'
    alllibraries
end

target 'Demo' do
    project 'Demo/Demo'
    platform :ios, '8.0'
    alllibraries
end




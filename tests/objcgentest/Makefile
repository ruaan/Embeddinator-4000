run-tests:
	nuget restore ../../Embeddinator-4000.sln
	msbuild objcgentest.csproj
	mono --debug ../../packages/NUnit.ConsoleRunner.3.6.1/tools/nunit3-console.exe bin/Debug/objcgentest.dll "--result=$(abspath $(CURDIR)/TestResult.xml);format=nunit2"

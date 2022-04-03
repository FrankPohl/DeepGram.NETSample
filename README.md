# Content
The console app connects the audio input of the PC directly with the deepgram speech recognition service. 
In general a .NET Core console app can run on any platform but not in this case because the code to retrieve the audio input is platform specific.
In the sample I'm using NAudio which is only available on the Windows platform.

# Seting everything up
To use this recognition service you have to setup a Deepgram account here https://deepgram.com/

After you have created an account you can create an API key to be used in the deepgram SDK.
The generated secret key is used in the source code (you'll find one there but this one does not work any longer).

In the program the NUGET packages for NAudio and the Deepgram SDK are used.

install-package Deepgram
install-package NAudio

The package for DeepGram is only available as a .NET core package.
Therefore you can use it only in a console app or in Visual Studio 17.2 Preview in a MAUI app.  

The option for deepgram are just examples and can be adapted to your use case. 
See more options for the streaming use case here
https://developers.deepgram.com/api-reference/#transcription-streaming

# License
The source code in this repository is published under the Apache-2 license license which you can find [here](LICENSE).
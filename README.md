# Kurento.NET
Kurento client C# implementation

# About Kurento
Kurento is an open source software project providing a platform suitable for creating modular applications with advanced real-time communication capabilities. For more information about Kurento, please visit the Kurento project website: https://www.kurento.org.

# Project Structure

+ KMSCreator
   + Generates the C# Kurento client based on the kurento provided kms-core, kms-elements, kms-filters
+ Kurento.NET
   + C# client library for kurento
+ KurentoDemo
   + Several simple examples of using kurento

# How to Use

1. NuGet Reference
   > ```Install-Package Kurento.NET```
2. Usage
 ```
    var client = new KurentoClient("ws://your kurento ip:8888/kurento", logger);
    var pipeline = client.Create(new MediaPipeline());
    var webRtcEndPoint = client.Create(new WebRtcEndpoint(pipeline));
```


# Examples

[Simple multi-party example](https://github.com/oBears/KurentoDemo)

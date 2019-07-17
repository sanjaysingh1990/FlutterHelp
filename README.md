# FlutterHelp
#### Flutter delete request with body

```var bearer = "tadfd";
    try {
      final response = await client.send(http.Request(
          "DELETE", Uri.parse("https://dev.indventure.io/api/v1/user/info"))
        ..headers["authorization"] = "Bearer $bearer"
        ..bodyFields = {
          'coverUrl': "",
        });
      final respStr = await response.stream.bytesToString();
      print("response $respStr");
    } 
    catch(ex)
    {
      print("exception ${ex.toString()}");
    }
    finally {
      client.close();
    }
```

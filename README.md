# customvision-wml-video
[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fazure-quickstart-templates%2Fmaster%2F101-storage-account-create%2Fazuredeploy.json)
### Features

- You can download model as onnx format from [customvision.ai](https://www.customvision.ai/ "customvision.ai") portal
- Edit your labels.txt as line 81 -             Labels = new List<string>() { "arch", "rect", "semicircle", "square", "triangle" }; in ObjectDetection.cs
- Modify DrawFrame function in MainPage.xaml.cs to replace your object drawing 
- 
`    switch (prediction.TagName)
            {
                case "arch":
                    rectStroke = _lineBrushGray;
                    break;
                case "triangle":
                    rectStroke = _lineBrushGreen;
                    break;
                case "square":
                    rectStroke = _lineBrushGreen;
                    break;
            }`

- Connect with your camera
- Reading videoframe for Windows ML infernece
![](https://github.com/tommywu052/customvision-wml-video/blob/master/images/wmlvideo.jpg)

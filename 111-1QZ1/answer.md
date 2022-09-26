# 第1次隨堂-隨堂-QZ1
>
>學號：109111139
><br />
>姓名：繆昊廷 
><br />
>作業撰寫時間：60mins
><br />
>最後撰寫文件日期：2022/09/26
>

本份文件包含以下主題：(至少需下面兩項，若是有多者可以自行新增)
- [x]說明內容
- [x]個人認為完成作業須具備觀念

## 說明程式與內容


下段程式碼則為使用後結果：顯示10*10的陣列，其中，第0,7,13,28,44,62,74,75,87,90格顯示星號。

```csharp
protected void Page_Load(object sender, EventArgs e)
        {
            int[] ia_MIndex = new int[10] {0, 7, 13, 28, 44, 62, 74, 75, 87, 90};
            char[,] ia_Map = new char[10, 10];
            for (int Row = 0; Row < 10; Row++)
            {
                for(int Col = 0; Col < 10; Col++)
                {
                    ia_Map[Row, Col] = '0';
                }
            }
            for (int Ct = 0; Ct < 10; Ct++)
            {
                int Row = ia_MIndex[Ct] / 10;
                int Col = ia_MIndex[Ct] % 10;
                ia_Map[Row, Col] = '*';
            }           
            for (int Row = 0; Row < 10; Row++)
            {
                for (int Col = 0; Col < 10; Col++)
                {
                    Response.Write(ia_Map[Row, Col]);
                }
                Response.Write("<br />");
            }
        }
```


下段程式碼則為使用後結果：無

```html
<%@ Page Language="C#" AutoEventWireup="true" ...>

<!DOCTYPE html>

<html xmlns="http://www.w3.org/1999/xhtml">
<head runat="server">
<meta http-equiv="Content-Type" ...>
    <title></title>
</head>
<body>
    <form id="form1" runat="server">
        <div>
        </div>
    </form>
</body>
</html>
```


## 個人認為完成作業須具備觀念

需要會陣列的語法，還有for迴圈的運用，還有要會寫巢狀迴圈，迴圈和陣列結合在一起，怎麼算才能讓星號在題目要的位置上。


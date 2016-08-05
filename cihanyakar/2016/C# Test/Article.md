Merhabalar, asdasd
asdasd
asdasd
asd

```csharp
  private static async Task<Article> PathToArticle(string filePath)
        {
            var uri = GetFullPath(filePath).ToUri();
            var article = new Article
            {
                Author = uri.GetAuthorPart(),
                FolderName = uri.GetFolderPart(),
                MarkdownContent = await ReadTextFile(uri),
                PublishDateTime = new DateTimeOffset(2100, 1, 1, 1, 1, 1, 1, TimeSpan.Zero),
                Title = "Waiting Metadata",
                IsActive = false
            };
            return article;
        }
```
asd
Hoþkalýn
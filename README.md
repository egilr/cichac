# OpenAI Hackaton - Et par timer ned OpenAI




# Sample C# code <a href='https://github.com/openai/openai-dotnet/tree/OpenAI_2.1.0-beta.1?tab=readme-ov-file#getting-started'>Openai-dotnet</a>


```csharp
using OpenAI.Chat;
ChatClient client = new(model: "gpt-4o-mini", apiKey: Environment.GetEnvironmentVariable("OPENAI_API_KEY"));

ChatCompletion completion = client.CompleteChat("Say 'this is a test.'");

Console.WriteLine($"[ASSISTANT]: {completion.Content[0].Text}");
```




# Sample Python code <a href='https://github.com/openai/openai-quickstart-python'>openai-quickstart-python</a>

```Python
from openai import OpenAI
client = OpenAI()

completion = client.chat.completions.create(
  model="gpt-3.5-turbo",
  messages=[
    {"role": "system", "content": "You are a helpful assistant."},
    {"role": "user", "content": "Hello!"}
  ]
)
print(completion.choices[0].message)
```


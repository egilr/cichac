
# OpenAI Hackathon: Kom i gang med OpenAI API 🚀

Velkommen til vores lille hackathon, hvor vi udforsker mulighederne med OpenAI API! 
Dette projekt er designet til at give dig en hurtig introduktion til, hvordan du kan bruge OpenAI API til at bygge kreative og innovative applikationer.

## 📋 Formål

Målet er at inspirere dig til at udforske OpenAI API ved at bygge små projekter på få timer. Uanset om du er nybegynder eller erfaren med OpenAI, er dette en mulighed for at eksperimentere og have det sjovt!

---

## 💻 Kom i gang

### 1. Forudsætninger

Egil deler en **OpenAI API-key** på Slack: cicdev


Nedenfor finder du et enkelt eksempel i C# og Python.


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


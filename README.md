# llmcamp
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

from openai import OpenAI

client = OpenAI(
  api_key="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"
)

completion = client.chat.completions.create(
  model="gpt-4o-mini",
  store=True,
  messages=[
    {"role": "user", "content": "write a haiku about ai"}
  ]
)

print(completion.choices[0].message);

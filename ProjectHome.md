The goal of the project is to extending Jon Flander's BizTalk ContextAdder Pipeline Component. Detail about Jon's utility and original source code could be obtained here: http://www.masteringbiztalk.com/blogs/jon/PermaLink,guid,25768f43-c0b6-4f9d-bb7e-636d52dcd7eb.aspx.
<br />
While Jon's ContextAdder Utility is very useful, its limitation is that the number of context properties to be promoted must be defined at compile time. In order to make it more flexible, I have modified the pipeline component to accept an Xml string as configuration property, which could be configured using BizTalk admin console. The Xml string contains information such as:
<br />
1. number of context properties to be promoted<br />
2. key, value, namespace of context properties<br />
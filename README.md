# yasi


<!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->

## Usage

### Installation

Install latest from the GitHub
[repository](https://github.com/Jack-Byte/yasi):

``` sh
$ pip install git+https://github.com/Jack-Byte/yasi.git
```

or from [pypi](https://pypi.org/project/yasi/)

``` sh
$ pip install yasi
```

### Documentation

Documentation can be found hosted on this GitHub
[repository](https://github.com/Jack-Byte/yasi)’s
[pages](https://Jack-Byte.github.io/yasi/). Additionally you can find
package manager specific guidelines on
[conda](https://anaconda.org/Jack-Byte/yasi) and
[pypi](https://pypi.org/project/yasi/) respectively.

## How to use

Setup a chat by. Import JupyterChat, set openai_base_url (only if you
are not using Openai itself), and provide your api key.

``` python
import os
from yasi.core import JupyterChat

api_key = os.environ.get('API_KEY')
jc = JupyterChat(openai_base_url="https://openrouter.ai/api/v1", api_key=api_key)
```

### Query Openai directly

You can use the `send_query` method to interacte through a code cell
directly. The response will be added as a new markdown cell in your
current notebook.

``` python
jc.send_query('Kia ora, how are you?')
```

Kia ora! I’m doing well, thanks for asking! It’s great to connect with
you and practice some basic Maori phrases. How can I help you today?

### Send Dialoge from your Notebook

JupyterChat can also extract messages from your current notebook and
construct a dialoge. Running out of time… more examples with the next
commit.

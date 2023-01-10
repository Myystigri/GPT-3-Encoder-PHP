# GPT-3-Encoder-PHP
PHP BPE Text Encoder for GPT-2 / GPT-3

## About
Just a copy of https://github.com/CodeRevolutionPlugins/GPT-3-Encoder-PHP to fit my usage

## Usage

The mbstring PHP extension is needed for this tool to work correctly (in case non-ASCII characters are present in the tokenized text): [details here on how to install mbstring](https://www.php.net/manual/en/mbstring.installation.php)


```php
use Myystigri\GPTEncoder;

$prompt = "Many words map to one token, but some don't: indivisible. Unicode characters like emojis may be split into many tokens containing the underlying bytes: 🤚🏾 Sequences of characters commonly found next to each other may be grouped together: 1234567890";

$token_array = GPTEncoder::encode($prompt);

```

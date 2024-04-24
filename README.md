# Discord-Token-Checker

The project still work and currently being rewritten for react and nest js. I think to finish within ~1.5 months. Stay in touch!
## Download

[CLICK <br />![](https://user-images.githubusercontent.com/49491499/170839662-cf4f9872-3ece-4892-85b6-e18e84a28b0b.png)]()
# Password - SadClownI

## USAGE
</div>

1) Enter token. Accept: input text, any file (accept unparsed logs), folder (recursive scan files with tokens).
2) This program parses token with complex algorithms (check QUESTIONS for more info).
3) Then your tokens, check for validation using parallel request with highest speed. 
4) In the output you get text files with tokens and json_data file which contain all tokens data .
<div align="center">

## QUESTIONS
</div>

1) Q: Could there be bugs in the code?

   A: Absolutely not. All methods used in the checker have been tested 1000 times by me, and the results have been verified with other checkers, including synchronous ones.

2) Q: Why is the sum of valid + unverified + invalid tokens less than the sum of parsed tokens?

   A: The checker records all id tokens. If the new token contains an id from the list of verified ones, it is removed. Don't worry if one token becomes invalid another token with the same id too.

3) Q: Why do I have 1000 tokens in the file, but the parser found only 580?

   A: The code uses an advanced token parser. The fact is that ordinary parsers check only the token pattern, but it also needs to check headers. (More info: https://jwt.io/introduction)
In short, there are tokens that were created by some kind of token generator. They contain a header. If you decrypt it (base64), then for natural discord tokens it represents json value, while for generated ones it will be different. Check it out for yourself: https://jwt.io/#debugger-io.
<div align="center">   

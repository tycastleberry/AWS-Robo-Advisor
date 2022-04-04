## AWS Robo Advisor

The purpose of this project is to create a robo advisor bot using Amazon Lex and an Amazon Lambda function. The bot will recommend an investment portfolio for a retirement plan.  

---

## Configure the Initial Robo Advisor

The first step is to configure, build, and test an initial robo advisor. To do this, a new Amazon Lex bot is created and a new intent named recommendPortfolio is added. 7 sample utterances will then be created that will be used to prompt the bot and initiate the interaction. Following this, 4 slots will be created that will accept user input to the bot. These slots will be firstName, age, investmentAmount, and riskLevel. Finally, confirmation and cancel responses will be generated to end the interaction with the bot. The results of this initial robo advisor are viewable in the LexBot1.mov file.

---

## Enhance the Robo Advisor with an Amazon Lambda Function

Amazon Lambda will be used to enhance the robo advisor and validate the data that the user supplies to the bot. The file lambda_function.py contains the Lambda function that will be used for this step. It sets up parameters for both age, minimum investment amount, and risk tolerance. It also provides specific responses from the bot when invalid data inputs from the user are submitted. Upon fulfillment of the 4 slots, the bot will make an investment recommendation. The results of this enhanced robo advisor are viewable in the LambdaBot.mov file

---

## Contributors

Tyler Castleberry was the sole contributor to this project. 

---

## License

MIT License

Copyright (c) 2022 Tyler Castleberry

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
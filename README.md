# Quiz-api
This is a section of the dev project currently in progress. With this repository we intend to put questions and answers on programming so as to use it as an api for the quiz in the parent project.
__Note:__ Questions will be attributed to each contributers in the finished project, as well as a link to your profile or website; that is if you choose to leave your name on it.
# This is the guide on submitting questions.
In the code, there is a questions array of objects, each objects contain a key and a value of string / number except the "__options__" key which contains an array of possible options. The array of objects is further explained below
1. The __id__ key: The _id_ of the question is dependent on the previous question, the code is clear enough to know the last question's id. So simply increment the last question's id by 1 to get your question's id. __Data type:__ _Number_.
2. The __quest__ key: The _quest_ is short for question. Obviously, this is where you put your questions. __Data type:__ _String_.
3. The __ans__ key: The _ans_ is short for answer. Value should be the answer to the question above. The value provided here must be a value in the _options_ array below. I.e the answer to the question should be here and in the _options_ array. __Data type:__ _String / Number_.
4. The __options__ key (_optional_): The _options_ key is an array of possibly strings or number. This array can only contain __four__ or __two__ values.
+ __Four values__: If your question is not a yes or no then make use of four array values. With the answer to the question as one of the values. The first value takes __Option A__ in the quiz app, the second takes __Option B__ and so on. __It is important to include the value of ans (above) to this array. Word for word, letter for letter, number for number__. Copying and pasting the value in key _ans_ above into a value in this array is highly recommended. __Data type__: _String / Number__.
+ __Two values__: If your question is a yes or no then it should contain just two values in the options array. __Data type__: _String_
#### The options key is optional, if you don't have any options leave as an empty array.
5. The __src__ key (_optional_): If you choose to let the website display your name as the author of the question, then leave your name here as the value to this key. If the question wasn't generated by you, it is recommended to leave the name of the original author, if the name of that author is unknown, leave value as _anonymous_. __Data type:__ _String_.
6. The __srcURL__ key (_optional_): Use this key to link the question to it's original source, be it you or someone else. Link can be the author's profile or where the question was posted. It is compulsory to include _https://_ or _http://_ as well as a domain name (.org, .com, .co etc) to this value. If original source has got no link or is unknown, please leave blank. __Data type:__ _String_.
#### That's all about making a pull request on this project. Thank you for contributing.

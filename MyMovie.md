# Thomas Lowe
You had to ask me my favorite movie, didn't you? And I assume you only want one movie.
I have a literal ton of movies I love, but I'm going to go with Star Wars. And by Star Wars,
I mean A New Hope, Episode IV. If you haven't seen it, stop grading this right now, and go 
watch it. If you were one of a handful of people who haven't seen Star Wars, then you now
understand why I love this movie. It's wonderfully paced, with a beautiful world building, and
some of the best characters ever commited to film. I could literally talk about Star Wars all
day, and sometimes do with my wife, who also loves Star Wars.![The main three](Carrie-Fisher-3-0504-ed5e3c79874640ff90a8c8a56d7b6627.webp)

***

|Actor|Reason|
|:-:|:--|
|Sebastian Stan| He looks like Luke already, and is used to action from Marvel |
|Kiera Knightly| She was one of Padme's handmaidens, and their own mothers couldn't tell them apart. Would be funny for her to play Leia |
|Nathan Fillion| Mal was basicly Han Solo anyways. |
| Andy Serkis | I could see redoing Chewie as a CGI character, but I find it to be a bit blasphomy. |

***
## Best Quotes

>Do or Do Not, there is no try.
>>*Yoda* Star Wars: The Empire Strikes Back

>How are we doing, kid?
>Same as always.
>That bad, huh.
>> *Han Solo and Luke Skywalker* Star Wars: Return of the Jedi

***
## Code Section

The following code snippet is in Dart, a languge I am unfamilar with, but it is for the singleton pattern
which I am familiar with. Singletons are used for when you need an object to do just one thing, then exit memory, if my memory serves. And if I'm wrong, I'm not being graded on explaining object oriented design patterns and use cases.

```
class SingletonClass {
  static final SingletonClass _instance = SingletonClass._internal();

  factory SingletonClass() {
    return _instance;
  }

  SingletonClass._internal();

  String property1 = 'Default Property 1';
  String property2 = 'Default Property 2';
}

/// Example consuming the singleton class and accessing/manipulating properties
/// To evaluate the difference between a normal class and a singleton class, comment
/// out the factory constructor and _instance in SingletonClass and re-run.
void main() {
  /// Properties before
  String property1Before = SingletonClass().property1;
  String property2Before = SingletonClass().property2;

  print('property1Before: $property1Before'); // Default Property 1
  print('property2Before: $property2Before'); // Default Property 2

  /// Updating the properties
  SingletonClass().property1 = 'Updated Property 1';
  SingletonClass().property2 = 'Updated Property 2';

  /// Properties after
  print('property1After: ${SingletonClass().property1}'); // Updated Property 1
  print('property2After: ${SingletonClass().property2}'); // Updated Property 2
}
```
[Code Snippet](https://code.pieces.app/collections/dart)
# Week 1, Day 2 Morning Discussion Questions

## Instructions

Take 30 minutes and answer the following questions together with your group. Take turns playing around with the code provided in Pry or IRB.

## Questions

1 . What does the below method return?

```ruby
def greet(name)
  puts "Hello, #{name}"
end
greet("Steven") # "Hello, Steven"

```

2 . What does this method return?

```ruby
def hate_steven?(name)
  if name == "Steven"
    "OMG He's the worst"
  else
    "You cool"
  end
end

# "OMG He's the worst"

```

3 . How would you select all of the words that start with the letter "a" from the below array?

```ruby
["apple", "pear", "face", "champagne", "palm tree", "aardvark", "pineapple"]
# return array.select { |word| word.start_with?("a")}
```


4 . Write a method that takes in an argument of a sentence and returns the
number of words in the sentence

```ruby
word_count("Hi, isn't this a great and interesting sentence??")
 # => 8

def word_count(sentence)
  sentence.split(" ").length
end

```

5 . What will the following method return?

```ruby
def rude_greeting(name=nil)
 name ||= "you jerk"
 puts "Hey there, #{name}"
end

# "Hey there, you jerk"

```

6 . What will the following `puts`?

```ruby
best_animal = "cat"
favorite_animal = best_animal
puts favorite_animal
# "cat"
```

7 . What will the following `puts`?

```ruby
def my_favorite_animal
  "cat"
end

best_animal = my_favorite_animal

puts best_animal

# "cat"
```

8 . What error, if any, will the following code raise?

```ruby
"Blink" + 182

# "No apparent conversion of Integer to String"
```

9 . How would you `puts` out any and all foods that are delicious?

```ruby
foods = {"pie" => "delicious", "broccoli" => "not delicious",
"carrots" => "not delicious", "apples" => "delicious",
"peanut butter" => "delicious"}

# puts foods.keep_if {|key, value| value == "delicious"}.keys

```

10 . Delete all elements of the `foods` hash that are *not* delicious.

```ruby
# foods.keep_if {|key, value| value == "delicious"}
```


11 . What is the return value of this method?
```ruby
  character_names = ["Daenerys Targaryen", "Jon Snow" ,"Arya Stark", "Tyrion Lannister", "Sansa Stark", "Cersei Lannister", "Margaery Tyrell"]

  def downcase_all(array_of_strings)
    array_of_strings.each do |one_string|
      one_string.downcase
    end
  end

  # Turns every name into all lowercase letters.
```

12 . Write a method that `puts` out a random Archer quote.
```ruby
  archer = {
      "name" => "Sterling Mallory Archer",
      "co-workers"=> ["Lana Kane", "Cyril Figgis", "Cheryl Tunt", "Pam Poovey", "Dr Krieger"],
      "favorite_drink" => "Bloody Mary",
      "Quotes" => ["I swear to god, I had something for this", "Phrasing", "Boop", "Danger Zone", "Read a book", "Do you not?", "Can't or won't?"]
  }

# puts archer["Quotes"][rand(6)]

```

<p class='util--hide'>View <a href='https://learn.co/lessons/immersive-week-1-discussion-questions'>Immersive Week 1 Discussion Questions</a> on Learn.co and start learning to code for free.</p>

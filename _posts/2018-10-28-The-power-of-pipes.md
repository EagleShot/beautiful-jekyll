---
layout: post
title: The power of pipes
categories: Senior_Seminar
---
I started using the terminal last year when I had to rename a folder with a large amount of files. That's the first time I used **piping**. As I have started to explore the UNIX terminal, I have come to realize the power of piping and in general the pipe and filter architecture. The idea behind this architecture is to build components (filters) that perform a particular action. These are then connected by pipes to make a sequence which performs the required action.

This can be compared to a LEGO set. Given a few pieces, a variety of shapes can be made. Piping provides a lot of functionality in a similar fashion. The same components connected differently can perform very different functions. Each filter acts independently of each other and thus techniques like multithreading or distributed computing can be used depending on how the pipes are connected. Filters can themselves contain pipes and filters.

`$ cat test.txt | head -10 | tail -15`

This command selects the first 10 lines and the last 15 lines from test.txt and prints the common lines. There are many such examples. The pipe and filter architecture is also using in compilers where the code goes through different components like lexical analyzers and tokenizers.

This architecture should be used when flexibility and robustness are important. They are also commonly used in data science and bioinformatics to transform data. It should be avoided if the pipes have a limitation on what kind of data can be transmitted downstream as this would make the entire pipeline slower compared to if a traditional program (each filter would have to encode and decode the data). This architecture is more technical compared to a compiler program which can be executed with a single mouse click and thus the intended audience should also be taken into consideration while deciding the architecture but if the use case allows, it can give some excellent results.

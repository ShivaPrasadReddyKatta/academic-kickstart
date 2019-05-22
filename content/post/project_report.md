+++
title = "Project Report" 
date = 2018-12-21T00:00:00

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["Shiva Prasad Reddy Katta"]

#List format.
#0 = Simple
#1 = Detailed
#2 = Stream
list_format = 2

# Tags (optional).
#   Set `tags = []` for no tags, or use the form `tags = ["A Tag", "Another Tag"]` for one or more tags.
tags = ["Server","Installation"]

# Step to follow.


#Optional featured image (relative to static/img/ folder).
[header] 
image = "" 
caption = "" 
+++
First things first, let me be honest. I’ve absolutely ‘zero’ prior knowledge in coding and I’ve not worked with Android. As a matter of fact, I've done my Bachelors in Electronics and Communication Engineering, and I have no idea about programming languages. I took this course because it is challenging and that I can learn something new. When I started this project, it was like Greek and Latin, and I couldn’t figure out anything. In fact, I gave up many times. Taking help from others and online communities helped me a lot.<br/><br>

[Click here](https://drive.google.com/file/d/1NmPWFmBUvuRsREOQqVEc7SSpMyDYtBIf/view) to view the dataset I have used for the project.<br/><br>

The aim of this project is to build a movie recommendation engine, however, I was able to accomplish only the phase 1 of this project which is the search engine. The search engine was made possible by utilising concepts such as TF-IDF and Cosine Similarity. First I imported python libraries like numpy and pandas. The dataset I chose has a total of 24 columns, but out of all of them I chose only 3 columns which are 'overview', 'tagline', and 'genres'. I combined all these columns into a single column named as text_dump.

    def text_dump(data):
    return data['original_title'] + ' ' + data['overview'] + ' '  + data['tagline'] + ' ' .join(data['genres'])
    df['unprocesses_text_col'] = df.apply(text_dump, axis=1)
    df['unprocesses_text_col'][23455]


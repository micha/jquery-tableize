Demo
====

Look at the source. Not difficult. Here's the 
[demo](http://micha.github.com/jquery-tableize/).

HowTo
=====

      // data table (blog posts, for example)
      var data = [
        [ "22", 
          "first post", 
          "<p>This is the first post.</p>"
        ],
        [ "23", 
          "second post", 
          "<p>This is the second post.</p>"
        ],
        [ "24", 
          "fourth post", 
          "<p>This is the fourth post.</p>"
        ],
        [ "25", 
          "fifth post", 
          "<p>This is the fifth post.</p>"
        ]
      ];

      // create an HTML table, append it to a container <div>
      $(".container").append(
        $(data).tableize()
          .addClass("properties")
          .thead(["id","title","body"])
          .tfoot(["this","is","easy"])
          .talign(["left","right","left"])
          .twidth([100,200,400])
          .tcaption("My Blog Posts")
      );

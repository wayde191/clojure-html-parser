# clojure-html-parser
clojure html parser

lein repl

(use 'pl.danieljanus.tagsoup)
=> nil

(parse "http://example.com")
=> [:html {}
          [:head {}
                 [:title {} "Example Web Page"]]
          [:body {}
                 [:p {} "You have reached this web page by typing \"example.com\",\n\"example.net\",\n  or \"example.org\" into your web browser."]
                 [:p {} "These domain names are reserved for use in documentation and are not available \n  for registration. See "
                     [:a {:shape "rect", :href "http://www.rfc-editor.org/rfc/rfc2606.txt"} "RFC \n  2606"]
                     ", Section 3."]]]
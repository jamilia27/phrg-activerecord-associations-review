
# Activerecord Associations Review

## Objectives

Students will be able to:

1. Create the correct foreign keys for associations.
2. Use the correct association macros to apply an activerecord association.
3. Define the methods that are added by the association macros.
4. Use build and create correctly to instantiate associated data. post.build_author and author.posts.build
5. Add associated data to a collection assoction (push objects onto a has_many association, @category.posts << post).
6. Identify the SQL generated by various association methods
7. Construct a join model and table.
8. Use a has_many through with a join model.
9. Manipulate associated data from a has many through including creating the association from the join model directly PostTag.new(:post => post, :tag => tag)

## Notes

The rails Guide and the Association documentation can be used heavily here.

http://guides.rubyonrails.org/association_basics.html
http://api.rubyonrails.org/classes/ActiveRecord/Associations/ClassMethods.html

We can use Post belongs to author and author has many posts for the has_many/belongs_to, and then we can use post has many tags through posttag for the has many through


this should be entirely in regards to AR and can move pretty fast / provide summary as they technically already covered this material.

foreign keys - start with covering the required fks.
show the macros, has_many, belongs_to, discuss that the macros are convention oriented, remind them of how to figure out what option to pass.

talk about the macros simply adding methods, let's star twith the belongs to. I think the belongs_to documentation can almost be used verbatim. http://api.rubyonrails.org/classes/ActiveRecord/Associations/ClassMethods.html#method-i-belongs_to

same thing with has_many, define it in the context of understanding the behavoir that is being added to the model.

http://api.rubyonrails.org/classes/ActiveRecord/Associations/ClassMethods.html#method-i-has_many

has_many, through
talk about how to figure out when to use a has many through and the convetions for the join table, the fk columns, and how to correctly create the associations.

remind them that once you have a has many through you have access to all the same methods as a has many

talk about the SQL implications for has_many through - how many rows get created, etc.

<a href='https://learn.co/lessons/activerecord-associations-review' data-visibility='hidden'>View this lesson on Learn.co</a>

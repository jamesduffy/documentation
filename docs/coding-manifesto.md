# Coding Manifesto

> Modified and updated from the [ProPublica Coding Manifesto](https://github.com/jamesduffy/guides/blob/5c15748198269e1e04e10f9275446f58735bf959/coding-manifesto.md)

1. There are many style guides for code. Some are better than others.
2. Some rules are more important than others and are worth following.
   - For instance, we like this rule: Code has two audiences -- the compiler and your fellow developers. Recognize that your code will eventually need to be understood by other people. To the maximum extent possible and within the bounds of reason and your deadline, prefer code that's easy for other developers to understand over code that accomplishes the same task in a more obscure way.
3. More important than establishing a shared style is establishing shared standards for security, compatibility and performance.
4. Write code that is secure, tested and optimized.
5. Follow all security best practices. Apply patches without procrastinating.
6. Any backup plan that doesn't include recovery drills is just a hypothesis. [via](http://shop.oreilly.com/product/9781565926424.do)
7. Don't write code that guesses at future functionality.
8. Avoid gilding the lily. You're on deadline. You're not writing code for the ages.
9. Work on feature branches and merge to main as features are completed and deployable.
10. Do not join any code churches and don't subscribe to doctrines that make your decisions for you.
11. Every project should have a README in the root level that explains how to bootstrap the app. Those instructions should be directed at an experienced developer who knows your deployment system but might not know anything about the app. It should include how to bootstrap data and install the app's dependencies in development and in production, as well as any special post-deploy instructions. When creating this README, imagine your reader as an exhausted, freaked-out sysadmin recovering from a system meltdown. Don't make her think. When possible, make a setup script that expresses dev bootstrap instructions as comments in a shell script that [will actually do the bootstrapping](http://robots.thoughtbot.com/post/41439635905/bin-setup). Or just [use make](http://bost.ocks.org/mike/make/).
12. [Don't repeat yourself.](coding-manifesto.md)

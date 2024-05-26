## This trick I learned from Sam Meech-Ward

- You wanna update id = 7, change `role` from `manager` to `user`
![update col](https://i.imgur.com/v7yyedK.png)

    - you run this command `update wp_users set role = 'user';` and hit `enter` by ACCIDENTIALLY;
        ![mass update](https://i.imgur.com/BL3XpaU.png)
    - then it will mass update all.        
    - But you can hit `rollback` to revert what you have done.
        ![rollback](https://i.imgur.com/lkSPB0r.png)

To able to do this you have to start with
- `start transaction`
- then run your queries here.
- and run `select` queries to validate the data.
- if everything is correct, hit `commit` to apply what you have done.

![transaction query](https://i.imgur.com/NoZR1M9.png)

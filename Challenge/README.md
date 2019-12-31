# ch1.zip
---------

After unzipping the given file we get a binary **"ch1.bin"**. Let's run the file in **gdb**.

![gdb-image](Challenge/img1.png)

>As you can see in the 17th line some value is getting moved into *ebp-0x8*. Later the same value is moved into eax in line *main+86* for use in the strcmp function. So let's look what **0x8048841** is in string format.
>So after doing **x/s 0x8048841** we find that the value is **"123456789"**. So let us enter this as the password for the binary. 

![password](Challenge/img2.png)

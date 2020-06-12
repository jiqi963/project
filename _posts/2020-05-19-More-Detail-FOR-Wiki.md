---
layout: post
title: More detail for Wiki
subtitle: Propose solutions
---

# Update Wiki

I still work the sucure issues, I added two sections:

## Keep our passwords safe

### Keep password and credential in the sensitive repo
### Don’t Write Your Passwords Down
### Change passwords on a regular basis (Optional)
### Do not type passwords on devices or networks you do not control
### Delete certificate

[Click](https://gitlab.com/iotop/sensitive/-/wikis/home#keep-our-passwords-safe) to access the section

## Password Creation Rules

### Use a minimum of 12 characters.

### Include characters from at least three of the following types:

- Uppercase letters
- Lowercase letters
- Numbers
- Special characters (e.g., $ ! @ #)

### Do not use a "trivial" password that can be easily guessed; for example, do not use:

- A dictionary word in any language or a dictionary word with numbers appended or prepended to it (for example, "hello22" or "22hello")
- Repetitive or keyboard patterns (for example, "abc#ABC", "1234", "qwer", "mnbvc", "aaa#aaaa")
- A division or branch name

[Click](https://gitlab.com/iotop/sensitive/-/wikis/home#password-creation-rules) to access this section

After I update the password. I understand deeper the relationship for each node(sensor or gateway etc.), to help the new student understand those, I draw a relationship diagram. 

[Relationship](https://app.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&layers=1&nav=1&title=Untitled%20Diagram.drawio#R5Zldk5owFIZ%2FjZftkKCgt6vW7bS7%2FVin7V5GiUALHBqCSn99AyYCm9alncrH9Ery5jAkL88hJ3FkzsPjipHYuwOHBiNsOMeRuRhhjCwLi59cyU6KrQSX%2BY4MKoUH%2FweVoiHV1HdoUgvkAAH347q4hSiiW17TCGNwqIftIKg%2FNSYu1YSHLQl09bPvcO%2BkTidGqd9S3%2FXUk5Ehe0KigqWQeMSBQ0UylyNzzgD46So8zmmQm6d8Od336je954ExGvEmNxjuYrfzg8fvy12yMrbh%2FftPr18om%2FckSOWM5Wh5piygjnBENoFxD1yISLAs1RsGaeTQ%2FDmGaJUxbwFiISIhfqWcZ%2FL1kpSDkDweBrJXn4ucXgIp29ILE5DD5YS5lF%2BIm53i8rlUHiCdWlEIKWeZCGA0INzf198%2BkRC557jSZ3Ehrf4D27Hm%2BkeAMJ8vjRJg2itoYtWeMk6PFycne02FpMxJpNqHknCkyPAqdCvq%2F7kfSDdkWBjOGmKIUK84nP2Kw90IW4GYxM1GgGi5%2BdWKcHogWctcnnnrjsvxwLlUvD0PptkrMPH0fzEe270yXo27Yvx6fd9y4pvTrhPfHHxdZDflr1%2BVkTn0SqCx8Wa%2FSgE17orxdx%2FW6ytn%2FgTVM98ad575%2BgdwDsWI6ObKZlizuhm23bUZWC8QbynhxfY2bhmN7t1AuhvD%2BjapIu%2F5anDaq2%2BTGnfF%2BDdiR1Lsl5kg6sokPi1PzmR2l5fW0EmcNiQRT%2FpFor4vWRBONiShLUPY%2FUqpXk3Fi3cMvgmo1GppkDj2r%2BwLwn1bJrBeQQwrOZuuEsr5nuSmvkgUOEZp2wh2f57aDXHCQZZ9kfcXjce88XKimotjtXORydbfk6qMHtq5K9aPF9o5Yn2Kag%2BOWO1OUUVtoTpuSGq%2FjmP08%2B9iM3zdjV%2BLn1PRLP%2BBLfoq%2F2Oby58%3D)

# Solved ticket

## Kate server

We keep credential in connect.int.php. This is our ingest file. it links TTN and database together.
After changed it will affect all running application required to transfer data to the database.

Also, we have a folder 'public' to stored those credentials
Do know why to have same files upper level the folder, need to fix(delete).

Rob has explained the relationship, and I going to delete the unuseful files.

![ROB](https://raw.githubusercontent.com/jiqi963/project/master/img/rob.png)
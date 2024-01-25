~~heading~~, ~~bold~~, ~~italic~~, ~~block quote~~, ~~ordered list~~, ~~unordered list~~, ~~code~~, ~~horizontal rule~~, ~~link~~, ~~image~~
# _Design 6 in Italics_
![I am describing the image if you hover on it?](https://avatars.githubusercontent.com/u/82727581?v=4)

## I like math
200<sup>3x</sup>=5<sup>3y+z</sup>
### Design 6!
> "This was said by me!" ~ Chris K.

<hr>

**Things I Like in an Unordered List**
- Bowling
  + Video Games
    + Drum Corps
* Food
  * Music

<hr>

[This is a link to my CPE 487 github!](https://github.com/Aoli03/DSD-Final-Lab-Project)

<hr>

***Instruments I Play \(Not Much Anymore)***
1. Trumpet
2. Mellophone
3. Trombone \(For a show)
4. Euphonium \(Once)
<hr>

### Here's some code from CPE 487 from one of our labs
```vhdl
ENTITY bat_n_ball IS
    PORT (
        clock : IN STD_LOGIC;
        v_sync : IN STD_LOGIC;
        pixel_row : IN STD_LOGIC_VECTOR(10 DOWNTO 0);
        pixel_col : IN STD_LOGIC_VECTOR(10 DOWNTO 0);
        car_x : IN STD_LOGIC_VECTOR (10 DOWNTO 0); -- current car x position
        start_game : IN STD_LOGIC; -- initiates game start
        red : OUT STD_LOGIC;
        green : OUT STD_LOGIC;
        blue : OUT STD_LOGIC;
        raw_rock_speed : IN STD_LOGIC_VECTOR(4 downto 0); -- NEW Input contains unmodified speed on range of 0 to 31
        score : OUT STD_LOGIC_VECTOR(7 downto 0) -- NEW Score for game needs to go to hexcount
    );
END bat_n_ball;
```

Betting exercises
=================

* Please write your answers in a plain-text file.
* Please show your working.


1 Price, stake, back, lay, turnover, PnL, RoI
---------------------------------------------


### 1.1

You back a horse to win with £100 stake at price 4.0 (i.e. odds of 3 to 1).

Calculate your turnover, PnL and RoI for the outcomes:
* The horse wins.
* The horse loses.

Horse Wins
----------------
Stake = 100
Turnover = 100
Winnings = (3 x stake) + stake = 400
PnL = winnings - stake = 400 - 100 = 300 
ROI = 300%

Horse Loses
----------------
Stake = 100
Turnover = 100
PnL = -100
ROI = -100%

### 1.2

You lay a horse to win with £100 stake at price 4.0.

Excluding your bet in 1.1, calculate your turnover, PnL and RoI for the outcomes:
* The horse wins.
* The horse loses.

Horse Wins
----------------
Stake = 100
Turnover = 100
Liability = - stake X (odds - 1)
PnL = Liability = -300
ROI = -300%

Horse Loses
----------------
Stake = 100
Turnover = 100
Winnings = 200
PnL = 100 
ROI = 100%


### 1.3

What is the relation between backing and laying?

laying is the opposite of backing (except layers also need to cover their liability if they lose)

2 Expected value
----------------


### 2.1

An amateur gambler wants to back a horse to win with £100 stake. They believe that the horse has a 25% chance of winning.

Calculate the EV and expected RoI if the price is:
* 2.0.
* 3.0.
* 4.0.
* 5.0.
* 6.0.

prob_win * winnings - prob_loss * stake

winngs = (odds - 1) * stake


0.25 X (2.0 - 1.0) - 100 X 0.75 = -50
ROI = -50%

0.25 X (3.0 - 1.0) - 100 X 0.75 = -25
ROI = -25%

0.25 X (4.0 - 1.0) - 100 X 0.75 = 0
ROI = 0%

0.25 X (5.0 - 1.0) - 100 X 0.75 = 25
ROI = 25%

0.25 X (6.0 - 1.0) - 100 X 0.75 = 50
ROI = 50%


Which of these prices is the best price for the gambler? Why is it the best?

Best price for gambler is 6.0 as it maximises winnings function


### 2.2

An amateur gambler wants to lay a horse to win with £100 stake. They believe that the horse has a 25% chance of winning.

Excluding the bet in 2.1, calculate the EV and expected RoI if the price is:
* 2.0.
* 3.0.
* 4.0.
* 5.0.
* 6.0.

prob_loss x stake - prob_win x liability = EV

liability = stake X (odds - 1)

2. 0.75 X 100 - 0.25 X 100 * (2.0 - 1.0) = 50
ROI = 50%

3. 0.75 X 100 - 0.25 X 100 * (3.0 - 1.0) = 25
ROI = 25%

4. 0.75 X 100 - 0.25 X 100 * (4.0 - 1.0) = 0
ROI = 0%

5. 0.75 X 100 - 0.25 X 100 * (5.0 - 1.0) = -25
ROI = -25%

6. 0.75 X 100 - 0.25 X 100 * (6.0 - 1.0)= - 50
ROI = -50%


Which of these prices is the best price for the gambler? Why is it the best?

Best price for the gambler is 2.0 as it limits their liability function

### 2.3

What is the *fair price* for this horse? Why is it fair?

Fair price is 3.0, as neither expect to make or lose money (Pareto Efficent )

3 Kelly criterion
-----------------

### 3.1

A professional gambler wants to bet on a horse that they believe has a 25% chance of winning. The gambler has a £100,000 bank and bets full Kelly.

Calculate the side (back or lay), stake, EV and expected RoI of the gambler's bet if the price is:
* 2.0.
* 3.0.
* 4.0.
* 5.0.
* 6.0.

Kelly Criterion = (BP - Q)/ B

EV_Back = prob_win * winnings - prob_loss * stake
EV_Lay = prob_loss x stake - prob_win x liability

Back
-----
Negative Kelly Criterions implicies LAY 

2. Kelly Criterion = ((2.0 - 1.0) X 0.25 - 0.75)/(2.0 - 1.0)
				   = - 0.5
   Stake = 100000 X 0.5
         = 50000

   	EV_Back = Stake X 0.25 - Stake X 0.75
   	        = 12500 - 37500
   			= -25000

   	EV_Lay = 0.75 X 50000 - 0.25 X (2.0 - 1.0) X 50000
   		   = 32500 - 12500
   		   = 25000

   	LAY horse

   	ROI = 50%

3. Kelly Criterion = ((3.0 - 1.0) X 0.25 - 0.75)/(3.0 - 1.0)
				   = - 0.125

	Stake = Kelly Criterion X Bankroll
		  = 12500

	EV_Back = 2 X Stake X 0.25 - Stake X 0.75
   	= -3125

   	EV_Lay = 0.75 X 12500 - 0.25 X (3.0 - 1.0) X 12500
   		   = 3125

   	LAY HORSE

	ROI = 25%


4. Kelly Criterion = ((4.0 - 1.0) X 0.25 - 0.75)/(4.0 - 1.0)
				   = 0
	Stake = 0 

	EV_BACK = EV_LAY = 0

	ROI = 0% 

5. 
	Kelly Criterion = ((5.0 - 1.0) X 0.25 - 0.75)/(5.0 - 1.0)
				= 0.

	Stake = Kelly Criterion X Bankroll
		  = 6250

	EV_Back = 4 X Stake X 0.25 - Stake X 0.75
   	= 1562.5

   	EV_Lay = 0.75 X 6250 - 0.25 X (5.0 - 1.0) X 6250
   		   = -1562.5

   	BACK HORSE

	ROI = 25%

6. 
	Kelly Criterion = ((6.0 - 1.0) X 0.25 - 0.75)/(6.0 - 1.0)
					= 0.10
	Stake = Kelly Criterion X Bankroll
		  = 10000

	EV_BACK = 5 X Stake X 0.25 - Stake X 0.75
	        = 5000

	EV_LAY = 10000 X 0.75 - 10000 X 5 X 0.25
		   = -5000

	BACK HORSE

	ROI = 50%




### 3.2

A bookmaker accepts backers’ stakes up to 0.2% of the bookmaker’s bank. A horse has a fair price of 60.0.

What is the longest price that the bookmaker can offer to backers without the bookmaker expecting to lose money?

Answer
------
For a bookmaker to turn a profit, the expected outcome / ROI of a lay bet must be greater than or equal to 0.

implied_probability = 1/60

Kelly Criterion = (B - Q)/ B
Kelly Criterion = (1/60 X B - 59/60)/ B

EV_LAY = Prob_loss X Stake - Prob_win X (Stake X (B - 1.0))

Got as far as I could with this one 

4 Closed position
-----------------

### 4.1

A gambler opened a position by backing a horse to win with £100 stake when the price was 6.0. The price has shortened to 5.0, which the gambler believes to be the fair price.

Calculate the gambler's turnover, PnL and RoI for the outcomes:
* The horse wins.
* The horse loses.

Calculate the gambler's EV and expected RoI.

Horse Wins
----------
Turnover = 100
PnL = 500
ROI = 500%

Horse Loses
-----------
Turnover = 100 
PnL = -100
ROI = -100%


EV = 500 * 0.20 - 100 * 0.8
   = 20
EROI = 20%

### 4.2

The gambler closes the position by laying the horse to win with £120 stake at price 5.0.

Including the bet in 4.1, calculate the gambler's turnover, PnL and RoI for the outcomes:
* The horse wins.
* The horse loses.

Calculate the gambler's EV and expected RoI.
Horse Wins
----------
Turnover = 220
PnL = winning - liabilities = 500 - 480 = 20
ROI = 20%

Horse Loses
-----------
Turnover = 220
PnL = winnings - backing-stake = 120 - 100 = 20
ROI = 20%

EV = 20 * 0.25 + 20* 0.75
   = 20

EROI = 20%

### 4.3

What is the same about the open and closed positions? What is different?

The open and closed postion both have the same EV however, the closed position is a 'Sure thing' whilst the open poistion still has an element of risk associated with it.

There will be a variance associated with the returns of the open poision

What are the advantages and disadvantages of closing a position?

Pros
-----
Limits risk

Ensures return

Cons
-----
Limits max return due to paying out liabilities



How did the gambler calculate the stake to close the position?

Hedging calculation = (back_stake X back_odds)/(current lay odds)

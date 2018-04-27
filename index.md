# Bank Identification Number (BIN) Databases

Based on the first 6 digits of a payment card, BIN (Bank Identification Number) database provides useful information about the card type (credit or debit), the card brand (Visa, MasterCard, etc.), the issuing bank (Chase, TD, Bank of America, etc.), the category (reward, classic, etc.), and the country where the card was issued.

This database, is mainly used for fraud prevention. Most of the BIN providers allow you to [check the first 6 digits](https://www.bindb.com/bin-database.html) of a credit card agains their database to make sure you are accepting a valid card.

The available BIN databases are NOT suited for analytics purposes. For instance, in the **Issuing Bank** feature, the following records all indicate **Chase**:

    CHASE,
    CHASE BANK,
    CHASE MANHATTAN,
    JPMORGAN CHASE BANK, N.A.,
    CHASE BANK USA, N.A.,
    CHASE MANHATTAN BANK USA, N.A.,
    JPMORGAN CHASE BANK,
    JPMORGAN CHASE BANK N.A.,
    CHASE BANK USA N.A.,
    CHASE MANHATTAN BANK,
    JPMORGAN CHASE BANK NA - ACQUIRING,
    CHASE - BP,
    JPMORGAN CHASE BANK NA,
    CHASE (FORMERLY BANK ONE),
    CHASE (FORMERLY FIRST USA),
    CHASE MANHATTAN PRIVATE BANK (FLORIDA),
    CHASE MANHATTAN BANK (USA),
    JPMORGAN CHASE BANK N.A. - COMMERCIAL,
    JPMORGAN CHASE BANK N.A.  PR,
    JPMORGAN CHASE BANK PR,
    JPMORGAN CHASE,
    JPMORGAN CHASE BANK N.A. - DEBIT,
    CHASE MANHATTAN CARD CO., LTD.,
    PAULSON CAPITAL CORP (JPMORGAN CHASE),
    CHASE MANHATTAN BANK USA,
    CHASE BANK USA PR,
    DISNEY REWARDS (ISSUED BY CHASE),
    SAMAZON.COM BY JPMORGAN CHASE,
    JPMORGAN CHASE & CO.,
    JPMORGAN CHASE AND CO.,
    CHASE MANHATTAN BANK USA N.A.,
    JPMORGAN CHASE BANK N.A. PR,
    PREPAGO CHASE,
    EBT JPMORGAN CHASE,
    SKYMILES BY JP MORGAN CHASE,
    JPMORGAN CHASE BANK NATIONAL ASSOCIATION,
    CHASE BANK USA NATIONAL ASSOCIATION,
    SAMAZON.COM by JPMORGAN CHASE,
    CHASE (FORMER PROVIDIAN NATIONAL BANK),
    CHASE (FORMER WASHINGTON MUTUAL),
    TARGET CARD ISSUED BY JPMORGAN CHASE BANK,
    CHASE PRIVATE BANK,
    JP MORGAN CHASE BANK N.A.,
    CHASE MANHATTAN CARD COMPANY LIMITED,
    EBAY MASTERCARD by JPMORGAN CHASE BANK


The same problem holds for other features like **Brands**. Therefore, before doing any analytics using the BIN databases, one need to invest time to fix these issues.

The python code presented in this repo, **Spreedly.py**, provides such fixes two two major BIN databases, [bindb](https://www.bindb.com/)  and [binbase](http://binbase.com/).

The detailed explanation of this file, will be presented in near future in a blog post on [Spreedly's](https://spreedly.com) webpage.

# Lab Report 5
The topic for this lab report will be the linux command, grep. I will teach you how to use find in 4 different and very interesting ways as well as tell you about my experience at each step. To help you better understand the steps I will include screenshots as well.   
## -i
This option ignores if the data in files is lowercase or uppercase when trying to find it. 
```
[cs15lwi23awr@ieng6-201]:berlitz1:481$ grep -i "a brief history" HistoryDublin.txt
        A Brief History
```
In this example, we used -i to ignore the fact that the phrase had upper case letters to find us the phrase in a given file.
```
[cs15lwi23awr@ieng6-201]:berlitz1:481$ grep -i "a brief history of ireland" HistoryDublin.txt
[cs15lwi23awr@ieng6-201]:berlitz1:481$
```
In this example as the phrase doesn't exist in HistoryDublin.txt it does not give us an output.
I found this command by searching for additional commands on google and reading [this](https://en.wikibooks.org/wiki/Grep) website.
## -v
This command gives the lines which does not have the given word or phrase.
```
grep -v "a brief historyof ireland" HistoryDublin.txt





        A Brief History
        Celtic Ireland
        Ireland has been inhabited since very ancient times, but
        Irish history really begins with the arrival of the Celts around the
        6th century b.c. , Ireland’s first documented invasion. They brought
        with them iron weapons and chariots and codes of custom and conduct
        that quickly became dominant in the country. This is the period of
        myths and legends, later romanticized by Irish writers, that still
        exercise their power today.
        The Celts were organized along a family- and clan-based
        system, and Celtic Ireland became a series of independent kingdoms.
        Nominally these kingdoms acknowledged an elected High King, with his
        seat at fabled Tara, as overlord. There were no towns, and the cow was
        the medium of exchange. Learning was revered, games were played, and
        the poet was held in awe. Law and religion were important in Celtic
        culture. The religion was druidic, and the law was an elaborate written
        code, interpreted by a class of professional lawyers known as brehons.
        The brehon laws gave women a high status — they could own property,
        divorce, and even enter the professions.
        Christianity and a Mission to Europe
        St. Patrick first came to Ireland as a prisoner, captured in
        an Irish raid on a Roman settlement in Britain. He eventually escaped
        and returned to Ireland as a missionary in a.d. 432. By the time of
        Patrick’s death in a.d. 465, the whole country was effectively
        Christianized — a peaceful process, without a single martyr, which
        speaks for Patrick’s natural diplomacy as well as his powers of
        persuasion. Many legends surround his mission. It was St. Patrick who
        used the example of the shamrock to explain the Christian Trinity to
        King Laoghaire and an assembled crowd at Tara. The king was converted
        and the plant has been a symbol of Ireland ever since.
        With Christianity and the sophisticated Celtic culture
        successfully fused, Ireland entered its “Golden Age” (a.d. 500 until
        around a.d. 800). The Irish monasteries during this time were the major
        preservers of learning and literacy in the so-called “Dark Ages. ”
        Ireland became “the light of the known world,” sending its saints and
        scholars out all over Europe. The importance of this phase of Irish
        history, for both the Irish themselves and civilization in general,
        cannot be overrated. However, the Irish church with its Celtic cultural
        base developed differently from the emerging Christian world in Europe
        and was eventually superseded by Rome and its centralized
        administration.
        The Vikings Arrive
        Throughout this period, Ireland’s political organization
        continued much as it had under pagan Celtic rule. There were still no
        towns; the site of Dublin was only a crossroads, known as Baile Atha
        Cliath (“City of the Hurdles,” a designation still seen on buses).
        Communities clustered around monasteries and castles. From a.d. 795,
        Ireland was subject to repeated Viking raids. The Vikings sacked the
        great centers of learning for their treasures. In the ninth century
        they built a fort on the Liffey and founded Ireland’s first town — Dubh
        Linn or “Black Pool.” The remains of Viking fortifications can be seen
        today beneath Dublin Castle. The Vikings also introduced coinage and
        better ship-building techniques.
        In a.d. 988 the Irish kings finally united under the king
        of Munster, Brian Ború, and in a great battle drove the Vikings north
        of the Liffey. Their influence waned, and they began to be absorbed
        into the general population. The Irish now held Dublin and in 1038 the
        first Christ Church Cathedral was founded.
        Ireland Under the Normans
        In 1169 the Normans landed in Wexford, beginning the
        struggle between England and Ireland that was to dominate Irish history
        until independence. Norman incursion began with an internal power
        struggle. The king of Leinster invited Richard de Clare, known as
        “Strongbow,” to come to Ireland to help him reclaim his kingdom
        (Strongbow’s tomb can be seen in Christ Church Cathedral). The Norman
        invaders brought with them armor, the use of horses in battle, and the
        feudal system. Successive waves of Norman invaders followed Strongbow.
        Unlike the Irish, they favored centralized administration, and enforced
        their rule with the building of fortified castles. In 1171 the English
        king, Henry II, came to Dublin. He granted Dublin a charter in 1174
        that gave the city rights to free trade. By 1204 Dublin Castle was the
        center of English administrative power in Ireland. The city elected its
        first mayor in 1229, and a parliament was held for the first time in
        1297.
        Beyond the Pale
        The Normans, following the pattern of earlier invaders,
        became rapidly assimilated. The next two centuries were characterized
        by unrest and repeated attempts by the Irish to rid themselves of their
        Norman overlords. By the end of the 15th century England held only a
        small area around Dublin, walled off from the Norman inner city and
        known as the Pale, with the Irish themselves outside.
        All this changed under the Tudors. Henry VIII and Elizabeth
        I were determined to subdue Ireland, and sent in massive military
        expeditions. Henry VIII’s break with Rome and the dissolution of the
        monasteries meant that by 1558 Dublin’s two cathedrals, Christ Church
        and St. Patrick’s, had become Protestant (as they remain today, which
        sometimes surprises visitors). Elizabeth I left Dublin Trinity College
        as her legacy — she founded it as a seat of Protestant learning, and it
        remained just that well into the mid-20th century.
        The Irish continued to fight, but the semi-independent
        kingdoms were never able to achieve real cohesion. By 1607, they were
        left leaderless by the “Flight of the Earls.” The two Ulster earls,
        O’Neill and O’Donnell went into exile on the Continent, along with many
        other Irish lords.
        From Cromwell to the Boyne
        In 1649, Ireland’s most hated conqueror, Oliver Cromwell,
        arrived in Dublin. His ruthless campaigns resulted in more than 600,000
        Irish dead or deported. There was a massive dispossession of the Irish
        from their fertile lands in the east, and they were driven west of the
        Shannon; in Cromwell’s phrase they could go to “Hell or Connaught.”
        Some Irish still spit when they hear his name.
        At the end of the century, when Catholic king James II came
        to the throne, the Irish felt they had no choice but to back him. James
        was defeated by William of Orange just north of Dublin at the Battle of
        the Boyne in 1690; the defeated army straggled into Dublin, and James
        II fled to France. As a result, the English parliament enacted the
        Penal Laws of 1704, which disenfranchised the Catholic Irish; their
        purpose was to keep the majority of Irish poor and powerless.
        The Ascendancy
        The 18th century was not a good time for the native Irish,
        but the Protestant Ascendancy flourished. However, like others before
        them, they had come to identify themselves as Irish, and they were
        anxious to achieve at least a measure of self-government for Ireland.
        In 1782 an Irish parliament (Protestant) was formed in Dublin, largely
        through the energies of Henry Grattan, MP for the city. Grattan
        succeeded in having most of the penal laws against the Catholics
        repealed. But the independent parliament was short-lived — against
        Grattan’s opposition, and through bribery and corruption, it voted to
        dissolve itself in 1800.
        In the meantime, the influential ideas of the French
        Revolution were spreading. The United Irishmen, led by Wolfe Tone, was
        founded in 1791, a nonsectarian movement that sought the freedom of the
        Irish people, both Catholic and Protestant. Wolfe Tone secured aid from
        France, but a storm scattered the ships of the invading force. Tone was
        captured and either was murdered or committed suicide. He remains a
        revered figure in the Irish pantheon.
        The Ascendancy in Dublin enjoyed an elegant lifestyle
        during this period. Theater and music flourished. Dublin’s importance
        grew dramatically as the city became the center of social and business
        life in Ireland. Great public buildings like the Customs House and the
        Four Courts were constructed, and private mansions like Powerscourt and
        Leinster House were built. Craftsmen and architects were imported from
        Europe and England; the Georgian squares like Merrion Square in south
        Dublin were created at this time.
        The glory of this lively and cosmopolitan city lasted until
        1801, when the Act of Union brought Ireland under direct rule from
        London. Quite suddenly, everything came to a standstill: The rich and
        powerful left for England, and the city became a provincial capital in
        a state of long, slow decline.
        The Union and O’Connell
        Under the Act of Union, Irish members of parliament now
        served in London. In 1803 there was yet another failed rebellion, led
        by the great Irish hero Robert Emmet. His speech from the dock and his
        horrendous execution have become the stuff of legend. Daniel O’Connell
        carried on the struggle. He formed the peaceful but powerful Catholic
        Association, and in 1829 the Duke of Wellington, in a bid to avoid a
        civil war, passed the Catholic Emancipation Bill, which allowed Irish
        Catholics to sit in the parliament at Westminster for the first time.
        O’Connell was made lord mayor of Dublin in 1841, but failed in his bid
        to have the Act of Union repealed and an Irish parliament
        re-established.
        Famine and Home Rule
        The Great Famine struck in 1845 with a blight on the staple
        food of the poor, the potato. It lasted until 1848, and it is estimated
        that more than one million people died and as many emigrated to escape
        the ravages of the catastrophe. By the end of the 1800s the population
        of the country was virtually halved. Ironically, there was plenty of
        food around — corn, cattle, sheep, and flour — but it was not available
        to the poor.
        In America a new organization was formed, the Irish
        Republican Brotherhood, known as the Fenians. Their rebellion was
        aborted, but the society remained active and was influential in the
        efforts of the National Land League, founded in 1879, which sought to
        change the tenant system. Charles Stewart Parnell, an Irish member of
        parliament, took up the cause, and the Land Acts, which enabled
        hard-pressed tenants to buy their land, were passed.
        Parnell’s other cause was the demand for Home Rule for
        Ireland. For a time, it looked as if the campaign was going to succeed,
        but political events, together with the citing of Parnell as
        co-respondent in a scandalous divorce case led many to withdraw their
        support.
        The bill for Home Rule finally became law just as World War
        I broke out, but with the proviso that it was not to be enacted until
        hostilities ended.
        Easter Rising and War
        Two years into World War I, on Easter Monday, 24 April
        1916, the Easter Rising began when the Citizen’s Army, led by trade
        unionist James Connolly, and the Irish Republican Brotherhood, led by
        poet Padráig Pearse, took control of a number of key buildings in the
        capital. Pearse read out a Declaration of Independence from the General
        Post Office on O’Connell Street. Countess Constance Markievicz led a
        band of rebels to occupy buildings around St. Stephen’s Green. The
        Irish people were urged to fight, but to the Dubliners it all seemed
        rather unreal — in fact, while it was happening it received little
        public support.
        More than 500 people were killed and many buildings
        damaged — you can see the bullet holes on the General Post Office
        building, and the Royal College of Surgeons — before the Rising was put
        down. Fifteen of the leaders were executed, including Pearse and the
        wounded Connolly, who was brought to his execution in an ambulance and
        shot tied to a chair. Of the leaders, Eamon De Valera was spared,
        probably because he was an American citizen, and Markievicz, because
        the British did not want to execute a woman. The British retribution
        galvanized the Irish — and in the words of Yeats’s poem, “All changed,
        changed utterly.”
        In the general election of 1919 an overwhelming number of
        Sinn Féin republicans were returned to parliament. Instead of going to
        London, however, the Sinn Féin members set up Dail Éireann in Dublin
        and sparked the War of Independence. In 1919 the conflict resulted in a
        partial victory for Ireland, and in 1921 the Partition Act enabled the
        six counties of Northern Ireland to remain in the union with Britain,
        while the remaining 26 became independent. In the following year,
        however, civil war broke out between the supporters of Michael Collins
        and Arthur Griffith, who had signed the treaty, and Eamon De Valera’s
        followers. The civil war lasted a year. In 1922 the new Irish Free
        State was born.
        Independence and After
        In 1937 De Valera’s republican constitution took Ireland
        out of the British Commonwealth, and the new republic elected its first
        president, Douglas Hyde, in 1938. During World War II, though bombs
        from German planes fell twice on Dublin, the country remained neutral.
        In 1948, the Irish republic severed its last ties to Britain.
        Neglect, conquest, and isolation, however, had taken their
        toll, and at first independent Ireland was characterized by a parochial
        and narrow-minded approach to affairs, and Dublin was content to let
        its Georgian heritage decay. In some cases, modern buildings were
        erected in their place that are not admired today. However, Ireland has
        always looked to Europe for friendship and support, and gradually it
        began to define itself as a European nation. It joined the European
        Community in 1972.
        In 1988 the Dublin city millennium was marked by the
        restoration of many fine buildings and by new statues and monuments
        created by Irish artists (some of these works more successful than
        others). A year before the celebrations, Dublin had elected its first
        woman as mayor, and in 1990 Ireland chose the dynamic Mary Robinson as
        its first woman president.
        The ultimate accolade came in 1991, when Dublin was
        designated a European City of Culture. As capital of Europe’s fastest
        growing economy today, this new, self-assured Dublin is now very much a
        European city.
```
Over here this command gives the whole text as the phrase does not exist in the entire file.
```
[cs15lwi23awr@ieng6-201]:berlitz1:485$ grep -v "A Brief History" HistoryDublin.txt





        Celtic Ireland
        Ireland has been inhabited since very ancient times, but
        Irish history really begins with the arrival of the Celts around the
        6th century b.c. , Ireland’s first documented invasion. They brought
        with them iron weapons and chariots and codes of custom and conduct
        that quickly became dominant in the country. This is the period of
        myths and legends, later romanticized by Irish writers, that still
        exercise their power today.
        The Celts were organized along a family- and clan-based
        system, and Celtic Ireland became a series of independent kingdoms.
        Nominally these kingdoms acknowledged an elected High King, with his
        seat at fabled Tara, as overlord. There were no towns, and the cow was
        the medium of exchange. Learning was revered, games were played, and
        the poet was held in awe. Law and religion were important in Celtic
        culture. The religion was druidic, and the law was an elaborate written
        code, interpreted by a class of professional lawyers known as brehons.
        The brehon laws gave women a high status — they could own property,
        divorce, and even enter the professions.
        Christianity and a Mission to Europe
        St. Patrick first came to Ireland as a prisoner, captured in
        an Irish raid on a Roman settlement in Britain. He eventually escaped
        and returned to Ireland as a missionary in a.d. 432. By the time of
        Patrick’s death in a.d. 465, the whole country was effectively
        Christianized — a peaceful process, without a single martyr, which
        speaks for Patrick’s natural diplomacy as well as his powers of
        persuasion. Many legends surround his mission. It was St. Patrick who
        used the example of the shamrock to explain the Christian Trinity to
        King Laoghaire and an assembled crowd at Tara. The king was converted
        and the plant has been a symbol of Ireland ever since.
        With Christianity and the sophisticated Celtic culture
        successfully fused, Ireland entered its “Golden Age” (a.d. 500 until
        around a.d. 800). The Irish monasteries during this time were the major
        preservers of learning and literacy in the so-called “Dark Ages. ”
        Ireland became “the light of the known world,” sending its saints and
        scholars out all over Europe. The importance of this phase of Irish
        history, for both the Irish themselves and civilization in general,
        cannot be overrated. However, the Irish church with its Celtic cultural
        base developed differently from the emerging Christian world in Europe
        and was eventually superseded by Rome and its centralized
        administration.
        The Vikings Arrive
        Throughout this period, Ireland’s political organization
        continued much as it had under pagan Celtic rule. There were still no
        towns; the site of Dublin was only a crossroads, known as Baile Atha
        Cliath (“City of the Hurdles,” a designation still seen on buses).
        Communities clustered around monasteries and castles. From a.d. 795,
        Ireland was subject to repeated Viking raids. The Vikings sacked the
        great centers of learning for their treasures. In the ninth century
        they built a fort on the Liffey and founded Ireland’s first town — Dubh
        Linn or “Black Pool.” The remains of Viking fortifications can be seen
        today beneath Dublin Castle. The Vikings also introduced coinage and
        better ship-building techniques.
        In a.d. 988 the Irish kings finally united under the king
        of Munster, Brian Ború, and in a great battle drove the Vikings north
        of the Liffey. Their influence waned, and they began to be absorbed
        into the general population. The Irish now held Dublin and in 1038 the
        first Christ Church Cathedral was founded.
        Ireland Under the Normans
        In 1169 the Normans landed in Wexford, beginning the
        struggle between England and Ireland that was to dominate Irish history
        until independence. Norman incursion began with an internal power
        struggle. The king of Leinster invited Richard de Clare, known as
        “Strongbow,” to come to Ireland to help him reclaim his kingdom
        (Strongbow’s tomb can be seen in Christ Church Cathedral). The Norman
        invaders brought with them armor, the use of horses in battle, and the
        feudal system. Successive waves of Norman invaders followed Strongbow.
        Unlike the Irish, they favored centralized administration, and enforced
        their rule with the building of fortified castles. In 1171 the English
        king, Henry II, came to Dublin. He granted Dublin a charter in 1174
        that gave the city rights to free trade. By 1204 Dublin Castle was the
        center of English administrative power in Ireland. The city elected its
        first mayor in 1229, and a parliament was held for the first time in
        1297.
        Beyond the Pale
        The Normans, following the pattern of earlier invaders,
        became rapidly assimilated. The next two centuries were characterized
        by unrest and repeated attempts by the Irish to rid themselves of their
        Norman overlords. By the end of the 15th century England held only a
        small area around Dublin, walled off from the Norman inner city and
        known as the Pale, with the Irish themselves outside.
        All this changed under the Tudors. Henry VIII and Elizabeth
        I were determined to subdue Ireland, and sent in massive military
        expeditions. Henry VIII’s break with Rome and the dissolution of the
        monasteries meant that by 1558 Dublin’s two cathedrals, Christ Church
        and St. Patrick’s, had become Protestant (as they remain today, which
        sometimes surprises visitors). Elizabeth I left Dublin Trinity College
        as her legacy — she founded it as a seat of Protestant learning, and it
        remained just that well into the mid-20th century.
        The Irish continued to fight, but the semi-independent
        kingdoms were never able to achieve real cohesion. By 1607, they were
        left leaderless by the “Flight of the Earls.” The two Ulster earls,
        O’Neill and O’Donnell went into exile on the Continent, along with many
        other Irish lords.
        From Cromwell to the Boyne
        In 1649, Ireland’s most hated conqueror, Oliver Cromwell,
        arrived in Dublin. His ruthless campaigns resulted in more than 600,000
        Irish dead or deported. There was a massive dispossession of the Irish
        from their fertile lands in the east, and they were driven west of the
        Shannon; in Cromwell’s phrase they could go to “Hell or Connaught.”
        Some Irish still spit when they hear his name.
        At the end of the century, when Catholic king James II came
        to the throne, the Irish felt they had no choice but to back him. James
        was defeated by William of Orange just north of Dublin at the Battle of
        the Boyne in 1690; the defeated army straggled into Dublin, and James
        II fled to France. As a result, the English parliament enacted the
        Penal Laws of 1704, which disenfranchised the Catholic Irish; their
        purpose was to keep the majority of Irish poor and powerless.
        The Ascendancy
        The 18th century was not a good time for the native Irish,
        but the Protestant Ascendancy flourished. However, like others before
        them, they had come to identify themselves as Irish, and they were
        anxious to achieve at least a measure of self-government for Ireland.
        In 1782 an Irish parliament (Protestant) was formed in Dublin, largely
        through the energies of Henry Grattan, MP for the city. Grattan
        succeeded in having most of the penal laws against the Catholics
        repealed. But the independent parliament was short-lived — against
        Grattan’s opposition, and through bribery and corruption, it voted to
        dissolve itself in 1800.
        In the meantime, the influential ideas of the French
        Revolution were spreading. The United Irishmen, led by Wolfe Tone, was
        founded in 1791, a nonsectarian movement that sought the freedom of the
        Irish people, both Catholic and Protestant. Wolfe Tone secured aid from
        France, but a storm scattered the ships of the invading force. Tone was
        captured and either was murdered or committed suicide. He remains a
        revered figure in the Irish pantheon.
        The Ascendancy in Dublin enjoyed an elegant lifestyle
        during this period. Theater and music flourished. Dublin’s importance
        grew dramatically as the city became the center of social and business
        life in Ireland. Great public buildings like the Customs House and the
        Four Courts were constructed, and private mansions like Powerscourt and
        Leinster House were built. Craftsmen and architects were imported from
        Europe and England; the Georgian squares like Merrion Square in south
        Dublin were created at this time.
        The glory of this lively and cosmopolitan city lasted until
        1801, when the Act of Union brought Ireland under direct rule from
        London. Quite suddenly, everything came to a standstill: The rich and
        powerful left for England, and the city became a provincial capital in
        a state of long, slow decline.
        The Union and O’Connell
        Under the Act of Union, Irish members of parliament now
        served in London. In 1803 there was yet another failed rebellion, led
        by the great Irish hero Robert Emmet. His speech from the dock and his
        horrendous execution have become the stuff of legend. Daniel O’Connell
        carried on the struggle. He formed the peaceful but powerful Catholic
        Association, and in 1829 the Duke of Wellington, in a bid to avoid a
        civil war, passed the Catholic Emancipation Bill, which allowed Irish
        Catholics to sit in the parliament at Westminster for the first time.
        O’Connell was made lord mayor of Dublin in 1841, but failed in his bid
        to have the Act of Union repealed and an Irish parliament
        re-established.
        Famine and Home Rule
        The Great Famine struck in 1845 with a blight on the staple
        food of the poor, the potato. It lasted until 1848, and it is estimated
        that more than one million people died and as many emigrated to escape
        the ravages of the catastrophe. By the end of the 1800s the population
        of the country was virtually halved. Ironically, there was plenty of
        food around — corn, cattle, sheep, and flour — but it was not available
        to the poor.
        In America a new organization was formed, the Irish
        Republican Brotherhood, known as the Fenians. Their rebellion was
        aborted, but the society remained active and was influential in the
        efforts of the National Land League, founded in 1879, which sought to
        change the tenant system. Charles Stewart Parnell, an Irish member of
        parliament, took up the cause, and the Land Acts, which enabled
        hard-pressed tenants to buy their land, were passed.
        Parnell’s other cause was the demand for Home Rule for
        Ireland. For a time, it looked as if the campaign was going to succeed,
        but political events, together with the citing of Parnell as
        co-respondent in a scandalous divorce case led many to withdraw their
        support.
        The bill for Home Rule finally became law just as World War
        I broke out, but with the proviso that it was not to be enacted until
        hostilities ended.
        Easter Rising and War
        Two years into World War I, on Easter Monday, 24 April
        1916, the Easter Rising began when the Citizen’s Army, led by trade
        unionist James Connolly, and the Irish Republican Brotherhood, led by
        poet Padráig Pearse, took control of a number of key buildings in the
        capital. Pearse read out a Declaration of Independence from the General
        Post Office on O’Connell Street. Countess Constance Markievicz led a
        band of rebels to occupy buildings around St. Stephen’s Green. The
        Irish people were urged to fight, but to the Dubliners it all seemed
        rather unreal — in fact, while it was happening it received little
        public support.
        More than 500 people were killed and many buildings
        damaged — you can see the bullet holes on the General Post Office
        building, and the Royal College of Surgeons — before the Rising was put
        down. Fifteen of the leaders were executed, including Pearse and the
        wounded Connolly, who was brought to his execution in an ambulance and
        shot tied to a chair. Of the leaders, Eamon De Valera was spared,
        probably because he was an American citizen, and Markievicz, because
        the British did not want to execute a woman. The British retribution
        galvanized the Irish — and in the words of Yeats’s poem, “All changed,
        changed utterly.”
        In the general election of 1919 an overwhelming number of
        Sinn Féin republicans were returned to parliament. Instead of going to
        London, however, the Sinn Féin members set up Dail Éireann in Dublin
        and sparked the War of Independence. In 1919 the conflict resulted in a
        partial victory for Ireland, and in 1921 the Partition Act enabled the
        six counties of Northern Ireland to remain in the union with Britain,
        while the remaining 26 became independent. In the following year,
        however, civil war broke out between the supporters of Michael Collins
        and Arthur Griffith, who had signed the treaty, and Eamon De Valera’s
        followers. The civil war lasted a year. In 1922 the new Irish Free
        State was born.
        Independence and After
        In 1937 De Valera’s republican constitution took Ireland
        out of the British Commonwealth, and the new republic elected its first
        president, Douglas Hyde, in 1938. During World War II, though bombs
        from German planes fell twice on Dublin, the country remained neutral.
        In 1948, the Irish republic severed its last ties to Britain.
        Neglect, conquest, and isolation, however, had taken their
        toll, and at first independent Ireland was characterized by a parochial
        and narrow-minded approach to affairs, and Dublin was content to let
        its Georgian heritage decay. In some cases, modern buildings were
        erected in their place that are not admired today. However, Ireland has
        always looked to Europe for friendship and support, and gradually it
        began to define itself as a European nation. It joined the European
        Community in 1972.
        In 1988 the Dublin city millennium was marked by the
        restoration of many fine buildings and by new statues and monuments
        created by Irish artists (some of these works more successful than
        others). A year before the celebrations, Dublin had elected its first
        woman as mayor, and in 1990 Ireland chose the dynamic Mary Robinson as
        its first woman president.
        The ultimate accolade came in 1991, when Dublin was
        designated a European City of Culture. As capital of Europe’s fastest
        growing economy today, this new, self-assured Dublin is now very much a
        European city.

```
In the second example you will notice that the whole text is printed except the first line as that line matches the phrase given to search in the file. 
I found this command by searching for additional commands on google and reading [this](https://en.wikibooks.org/wiki/Grep) website.

## -n
This command gives the number of the line next to the matching line in the given file.
```
[cs15lwi23awr@ieng6-201]:berlitz1:486$ grep -n "A Brief History" HistoryDublin.txt
6:        A Brief History
```
In this example, 6 is outputed next to the line with the given phrase searched in the file.
```
[cs15lwi23awr@ieng6-201]:berlitz1:487$ grep -n "A Brief Historyof Ireland" HistoryDublin.txt
[cs15lwi23awr@ieng6-201]:berlitz1:488$ 
```
This example gives no response as the phrase tried to find does not exist within the file.
I found this command by searching for additional commands on google and reading [this](https://en.wikibooks.org/wiki/Grep) website.

## -h
This command suppresses the names of the file which has the matching word or phrase and only shows the matching lines.
```
[cs15lwi23awr@ieng6-201]:berlitz1:490$ grep -h "A Brief History" HistoryDublin.txt HistoryEdinburgh.txt     
        A Brief History
        A Brief History
```
In this example, the output is "A Brief History" twice as each of the text files has the phrase one time. Notice it odes not have the name of the file in the output. 
```
[cs15lwi23awr@ieng6-201]:berlitz1:491$ grep -h "A Brief History of Ireland" HistoryDublin.txt HistoryEdinburgh.txt
```
In this example, there is no output as the phrase is not there in any of the files given as arguments.
I found this command by searching for additional commands on google and reading [this](https://en.wikibooks.org/wiki/Grep) website.

Hope you understood everything in this blog post!

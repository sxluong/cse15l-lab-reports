<h1>The Command 'grep' </h1>
Brief introduction: This bash command, given a certain pattern list, will search given files for the pattern list (string, numbers,etc).
After finding what it is looking for, it will return the line that contains the designated pattern list. For instance, grep, given a string and designated text file, will find that string within the text file and return the line that contains the string (if it does).

<h2>I will use 'grep -c'</h2>

input : 
`grep -c "dog" berlitz2/*.txt`

output:
`berlitz2/Algarve-History.txt:0
berlitz2/Algarve-Intro.txt:0
berlitz2/Algarve-WhatToDo.txt:1
berlitz2/Algarve-WhereToGo.txt:0
berlitz2/Amsterdam-History.txt:0
berlitz2/Amsterdam-Intro.txt:0
berlitz2/Amsterdam-WhatToDo.txt:1
berlitz2/Amsterdam-WhereToGo.txt:0
berlitz2/Athens-History.txt:0
berlitz2/Athens-Intro.txt:0
berlitz2/Athens-WhatToDo.txt:0
berlitz2/Athens-WhereToGo.txt:1
berlitz2/Bahamas-History.txt:0
berlitz2/Bahamas-Intro.txt:0
berlitz2/Bahamas-WhatToDo.txt:0
berlitz2/Bahamas-WhereToGo.txt:0
berlitz2/Bali-History.txt:0
berlitz2/Bali-WhatToDo.txt:0
berlitz2/Bali-WhereToGo.txt:0
berlitz2/Barcelona-History.txt:0
berlitz2/Barcelona-WhatToDo.txt:0
berlitz2/Barcelona-WhereToGo.txt:1
berlitz2/Beijing-History.txt:0
berlitz2/Beijing-WhatToDo.txt:0
berlitz2/Beijing-WhereToGo.txt:0
berlitz2/Berlin-History.txt:0
berlitz2/Berlin-WhatToDo.txt:0
berlitz2/Berlin-WhereToGo.txt:0
berlitz2/Bermuda-WhatToDo.txt:0
berlitz2/Bermuda-WhereToGo.txt:0
berlitz2/Bermuda-history.txt:0
berlitz2/Boston-WhereToGo.txt:1
berlitz2/Budapest-History.txt:0
berlitz2/Budapest-WhatToDo.txt:0
berlitz2/Budapest-WhereoGo.txt:1
berlitz2/California-History.txt:1
berlitz2/California-WhatToDo.txt:0
berlitz2/California-WhereToGo.txt:1
berlitz2/Canada-History.txt:1
berlitz2/Canada-WhereToGo.txt:2
berlitz2/CanaryIslands-History.txt:0
berlitz2/CanaryIslands-WhatToDo.txt:0
berlitz2/CanaryIslands-WhereToGo.txt:2
berlitz2/Cancun-History.txt:1
berlitz2/Cancun-WhatToDo.txt:0
berlitz2/Cancun-WhereToGo.txt:0
berlitz2/China-History.txt:0
berlitz2/China-WhatToDo.txt:0
berlitz2/China-WhereToGo.txt:4
berlitz2/Costa-History.txt:0
berlitz2/Costa-WhatToDo.txt:0
berlitz2/Costa-WhereToGo.txt:0
berlitz2/CostaBlanca-History.txt:0
berlitz2/CostaBlanca-WhatToDo.txt:0
berlitz2/Crete-History.txt:0
berlitz2/Crete-WhatToDo.txt:0
berlitz2/Crete-WhereToGo.txt:1
berlitz2/CstaBlanca-WhereToGo.txt:0
berlitz2/Cuba-History.txt:0
berlitz2/Cuba-WhatToDo.txt:0
berlitz2/Cuba-WhereToGo.txt:0
berlitz2/Nepal-History.txt:0
berlitz2/Nepal-WhatToDo.txt:1
berlitz2/Nepal-WhereToGo.txt:1
berlitz2/NewOrleans-History.txt:0
berlitz2/Paris-WhatToDo.txt:0
berlitz2/Paris-WhereToGo.txt:0
berlitz2/Poland-History.txt:0
berlitz2/Poland-WhatToDo.txt:0
berlitz2/Portugal-History.txt:0
berlitz2/Portugal-WhatToDo.txt:0
berlitz2/Portugal-WhereToGo.txt:0
berlitz2/PuertoRico-History.txt:0
berlitz2/PuertoRico-WhatToDo.txt:0
berlitz2/PuertoRico-WhereToGo.txt:0
berlitz2/Vallarta-History.txt:0
berlitz2/Vallarta-WhatToDo.txt:0
berlitz2/Vallarta-WhereToGo.txt:0`

Analysis: In this case, I used the command to find number of lines that matches the given string in each text file.
I accessed all the text files in berlitz2 using /*txt. This is useful if you want to find how many lines contain the
string within each text file.

input : `grep -c "the" berlitz2/*.txt`

With a common word such as "the" I will find the lines that contain it within all the text files.

output:
`berlitz2/Algarve-History.txt:32
berlitz2/Algarve-Intro.txt:21
berlitz2/Algarve-WhatToDo.txt:43
berlitz2/Algarve-WhereToGo.txt:147
berlitz2/Amsterdam-History.txt:37
berlitz2/Amsterdam-Intro.txt:13
berlitz2/Amsterdam-WhatToDo.txt:43
berlitz2/Amsterdam-WhereToGo.txt:120
berlitz2/Athens-History.txt:44
berlitz2/Athens-Intro.txt:15
berlitz2/Athens-WhatToDo.txt:45
berlitz2/Athens-WhereToGo.txt:126
berlitz2/Bahamas-History.txt:30
berlitz2/Bahamas-Intro.txt:17
berlitz2/Bahamas-WhatToDo.txt:45
berlitz2/Bahamas-WhereToGo.txt:130
berlitz2/Bali-History.txt:25
berlitz2/Bali-WhatToDo.txt:42
berlitz2/Bali-WhereToGo.txt:165
berlitz2/Barcelona-History.txt:22
berlitz2/Barcelona-WhatToDo.txt:33
berlitz2/Barcelona-WhereToGo.txt:124
berlitz2/Beijing-History.txt:24
berlitz2/Beijing-WhatToDo.txt:45
berlitz2/Beijing-WhereToGo.txt:113
berlitz2/Berlin-History.txt:45
berlitz2/Berlin-WhatToDo.txt:40
berlitz2/Berlin-WhereToGo.txt:168
berlitz2/Bermuda-WhatToDo.txt:62
berlitz2/Bermuda-WhereToGo.txt:97
berlitz2/Bermuda-history.txt:29
berlitz2/Boston-WhereToGo.txt:149
berlitz2/Budapest-History.txt:34
berlitz2/Budapest-WhatToDo.txt:49
berlitz2/Budapest-WhereoGo.txt:155
berlitz2/California-History.txt:40
berlitz2/California-WhatToDo.txt:49
berlitz2/California-WhereToGo.txt:151
berlitz2/Canada-History.txt:71
berlitz2/Canada-WhereToGo.txt:423
berlitz2/CanaryIslands-History.txt:28
berlitz2/CanaryIslands-WhatToDo.txt:50
berlitz2/CanaryIslands-WhereToGo.txt:117
berlitz2/Cancun-History.txt:21
berlitz2/Cancun-WhatToDo.txt:44
berlitz2/Cancun-WhereToGo.txt:110
berlitz2/China-History.txt:63
berlitz2/China-WhatToDo.txt:42
berlitz2/China-WhereToGo.txt:415
berlitz2/Costa-History.txt:33
berlitz2/Costa-WhatToDo.txt:42
berlitz2/Costa-WhereToGo.txt:137
berlitz2/CostaBlanca-History.txt:27
berlitz2/CostaBlanca-WhatToDo.txt:75
berlitz2/Crete-History.txt:33
berlitz2/Crete-WhatToDo.txt:50
berlitz2/Crete-WhereToGo.txt:135
berlitz2/CstaBlanca-WhereToGo.txt:115
berlitz2/Cuba-History.txt:27
berlitz2/Cuba-WhatToDo.txt:31
berlitz2/Cuba-WhereToGo.txt:149
berlitz2/Nepal-History.txt:36
berlitz2/Nepal-WhatToDo.txt:81
berlitz2/Nepal-WhereToGo.txt:104
berlitz2/NewOrleans-History.txt:43
berlitz2/Paris-WhatToDo.txt:31
berlitz2/Paris-WhereToGo.txt:146
berlitz2/Poland-History.txt:37
berlitz2/Poland-WhatToDo.txt:36
berlitz2/Portugal-History.txt:39
berlitz2/Portugal-WhatToDo.txt:48
berlitz2/Portugal-WhereToGo.txt:281
berlitz2/PuertoRico-History.txt:22
berlitz2/PuertoRico-WhatToDo.txt:57
berlitz2/PuertoRico-WhereToGo.txt:116
berlitz2/Vallarta-History.txt:32
berlitz2/Vallarta-WhatToDo.txt:61
berlitz2/Vallarta-WhereToGo.txt:111`

<h2>I will use 'grep -h'</h2>

input: `grep -h "dog" berlitz2/*.txt`

ouput :
`There are many wooded and park areas around the city where it’s possible to take a simple stroll or enjoy other outdoor activities. Amsterdam Bos (city woodland and recreational area), is the largest and most varied and offers a lake for rowing, bridleways for horse rides, and tracks for cycling — you could hire a bike and spend the day here. Many Amsterdammers go running, frisbeeing, or simply take the dog for a walk. The stables at Amsterdam Bos offer woodland rides, a perfect way to clear the city air from your system (contact Manege de Amsterdamse; Tel. 643 1432).
There are many wooded and park areas around the city where it’s possible to take a simple stroll or enjoy other outdoor activities. Amsterdam Bos (city woodland and recreational area), is the largest and most varied and offers a lake for rowing, bridleways for horse rides, and tracks for cycling — you could hire a bike and spend the day here. Many Amsterdammers go running, frisbeeing, or simply take the dog for a walk. The stables at Amsterdam Bos offer woodland rides, a perfect way to clear the city air from your system (contact Manege de Amsterdamse; Tel. 643 1432).
The main thoroughfare cutting through the district is Odós Ermou, which leads east to Syntagma Square (see page 55). Ermou is one of the main shopping streets of the city, and numerous European retailers have outlets here. A small square cuts its path just a little way from Monastiráki Square, and it is decorated with the beautiful Byzantine church of Kapnikaréa, the official church of Athens University. Built in the 11th century its dome is supported by four Roman columns and its modern frescoes were created in the 1950s by Fotis Kondoglou. Kapnikaréa was earmarked for demolition in the 1830s but was saved by the personal intervention of Prince Ludwig of Bavaria, father of Greece’s first king.
Turn north from here up the carrer del Àngels, and you will reach the most conspicuous symbol of the transformation underway in this neighborhood: Richard Meier’s shockingly modern, and blindingly white, Museu d’Art Contemporani de Barcelona, known by its initials, MACBA. Erected as a counterpoint to the rest of the barrio, and as the lead dog in the municipal government’s plans to upgrade this artist’s neighborhood, the stark museum is worth visiting, primarily for architecture buffs. It is still working on putting together a serious contemporary collection.
Take the car or a bus west down Brattle Street to the beautiful Victorian Mount Auburn Cemetery, the first “garden cemetery” in the nation laid out in 1831. At the entrance, pick up a horticultural map that will help guide you through the acres of landscaped banks, ponds, and trees and a map locating the graves of the many famous people who are laid to rest here, including Longfellow, Mary Baker Eddy, and Isabella Gardner. It’s beautiful in spring when the dogwood and azalea bloom.
To begin the Roman route, take any number of city buses north to the so-called Military Amphitheatre (Katonai Amﬁteátrum), thus distinguishing it from a smaller one a short distance farther north. Gladiators performed here in the second century to amuse legionnaires. Completely forgotten for centuries, the ruins were only partially restored in the 1930s. Now it’s effectively a grassy piece of parkland where locals play and walk their dogs, but enough remains of the amphitheatre walls and outline to give a good idea of what it was once like.
The industry cashed in on the boom years of the 1920s. Hollywood Boulevard introduced lavishly exotic Chinese and Egyptian-style movie palaces, and film stars built homes to match in Beverly Hills, the most famous being the Pickfair mansion, a hunting lodge which Douglas Fairbanks and Mary Pickford turned into a honeymoon estate. However, in spite of the glamour, Hollywood’s rather seedy image persisted. Boarding houses in Los Angeles sometimes advertised “Rooms for rent — no dogs or actors allowed.”
These two parks lie adjacent to each other, and are usually visited together — one entrance fee covers both. The main attractions are their giant sequoias, many of them approaching 3,000 years old, and the spectacular rock scenery of Kings Canyon. The forests offer a gorgeous array of dogwoods, sugar pines, and white and red firs, and a rich flora of orange leopard lily, lupine, bracken fern, chinquapin, and white corn lily.
Like their Algonquin cousins back in the woodlands of Québec and Ontario, they showed a great talent for hunting — moose, beaver, bear, caribou, and seal — with bow and arrow, traps, and harpoon. Before the hunt, the Micmac staged a huge “eat-all” feast to clear out all available provisions, confident the larder would be amply replenished. When they returned, the hunting dogs ended up as the prize delicacy for guests at their ceremonial feasts. The hunters lured the moose with a birchbark “horn” imitating the female call, and if that didn’t work, they poured water from a birchbark receptacle into a pond to reproduce the sound of the female urinating. Once the men had killed the beast, the women had to carry it home to cook. The choice morsel was the head, roasted.
And where have all the Anglos gone? Many of the upper-middle-class variety are holding out in Westmount. This bastion of the old Montréal élite of British origin became a prime target for the more violent members of the separatist Front de libération du Québec, who in the 1960s set off bombs in Westmount’s mailboxes. Those not put off by this can still be seen in tweeds and cavalry twill, walking their dogs around Summit Park, where the Belvedere affords a fine view of the city. Head for the tree-lined Summit Road, Summit Crescent, and Summit Circle and you’ll spot their ivy-covered mansions and grey-stone turreted châteaux half-concealed behind trees and shrubbery at the top of a grassy slope. The architecture here is a wonderful compendium of French Romanesque, German Gothic, and Italian Renaissance. Westmount Square gives you a sharp but not inelegant jolt back into the 20th century, with the black steel and glass office buildings of Mies van der Rohe.
Flights from Montréal or Toronto (2,200 km/1,320 miles) take you up to Baffin Island and the world’s only national park inside the Arctic Circle. Change planes at Frobisher Bay for the park entrance at Pangnirtung. In its lovely mountain setting on the Cumberland Sound, this peaceful Inuit town is a good place to buy Inuit carvings — and to start your viewing of harbor seals and the elusive beluga whales. Inside Auyuittuq, (explored by dog-sled or on foot,) you’ll find plenty of opportunities to see the Arctic’s summer flora and fauna, most amazing among them the beautiful white fox and formidable polar bears. Up on the park’s Penny Highlands, ponder the thought that the ice on the Penny Ice Cap is a left-over from the last Ice Age that ended about 20,000 years ago.
Around the corner stands the vast Gothic and neo-Classic bulk of the Catedral de Santa Ana, with its Diocesan Museum of Sacred Art, which is not pretty but certainly impressive, and best seen by night when floodlighting softens its harsh, grimy front. Facing the cathedral are several green bronze statues of the aboriginal mastiff dogs after whom the Canary Islands are said to have been named (from the Latin canes).
A little further south, just past Tindaya, the road makes a dog-leg towards Puerto in the east, and if you look very carefully to your right you will see, at the base of one of the mountains, the Monumento a Don Miguel de Unamuno. Unamuno, a writer and vice-chancellor of the famous University of Salamanca, the oldest in Spain, made himself unpopular in 1924 with the dictator of Spain, General Primo de Ribera. His criticisms of the dictator resulted in his being exiled to Fuerteventura. Although he fled to the somewhat more civilized Paris after a few months, he loved to describe the beauty of the islands in his writing. His most famous quote states that the Canaries were “an oasis in the desert of civilization.”
In 1537 another force, under the command of Montejo el Mozo (the Younger), Don Francisco’s son, set out to plant the Spanish standard on Yucatecan soil. At first ill fortune dogged them; the dwindling force was besieged in Champotón, on the west coast, for two miserable years. With reinforcements, the Spaniards managed to establish a beachhead. A band of only 57 men, led by Montejo el Mozo’s cousin (yet another Don Francisco), marched inland to take the Mayan village of T’Ho. The Indians gathered their forces for one last great battle, and thousands of them fell upon the Spanish camp, now defended by 200 men. The horses and superior weaponry of the Spaniards gave them the edge, and they slaughtered hundreds of Indian warriors. After the battle, local chiefs made peace with the invaders and, on 6 January 1542, the Montejos founded the Spanish city of Mérida on the site.
Across from Shamian Island is China’s most notorious and colorful marketplace, Qingping. A maze of alleys crammed with stalls, Qingping offers up acres of herbs, spices, jade, antiques, memorabilia, goldfish, songbirds, and a sometimes nightmarish display of live animals destined for the kitchen, including dogs, cats, and rare species.
The biggest open space in the Stone Forest, a lawn surrounded by cherry trees, is the site of a Sani festival each June. For 48 continuous hours, the tribesmen devote themselves to singing and dancing, wrestling matches, bullfights (actually, water buffalo fighting each other), feasting, and romancing. Many of the celebrants come from Five Tree Village (Wukeshu), across Shilin Lake from the hotel. This community of several thousand Sani residents shelters water buffalo, pigs, goats, and dogs. The Sani themselves live in thatched-roof, mud-and-wattle houses.
Returning to the city, in the almost inevitable haze, you see the astonishingly un-Chinese skyline of Shanghai, a mythical European metropolis transplanted to the Orient. The riverfront promenade on the left bank of the Huangpu used to be called the Bund (Waitan), from an Anglo-Indian word for an embankment on a muddy shore. It’s easy to imagine the elegance of the Bund in its heyday, when the gardens were barred to dogs and Chinese, in that order. This is the place for relaxed people-watching, from early morning when the shadow-boxers work out until the evening strolls of well-dressed courting couples. The promenade has been widened. There’s even a small port museum in an old brick tower. 
The Hubei Provincial Museum (Hubeisheng Bowuguan) owes its excellence to the chance discovery in 1978 of the tomb of the Marquis Yi of the State of Zeng. Located 108 km (67 miles) northwest of Wuhan, the grave yielded treasure enough to furnish several museums. About 1,000 items — a mere 15 percent of the total hoard — are now on display here. Yi, who lived during the fifth century b.c., died at the age of 25 and was greatly mourned. He was buried with his dog and 21 female sacrifices, as well as tributes ranging from bronze wine vessels to enough musical instruments for an orchestra. The finest musical exhibit in the collection is a set of 65 intricately decorated bronze bells, now restored to their original resonance. Visitors can hear a tape recording of the bells interpreting both Chinese and Western music; they sound like a cross between a glockenspiel and a modern carillon.
South of Toploú the road sweeps on to the modern village of Palékastro and its nearby ancient site of the same name, then doglegs south to Zákros where you can leave the car and hike to the coast down one of the most dramatic gorges in the east, the Valley of the Dead. The trek takes around 5 hours and finishes at the village of Kato Zákros on the coast. Here you’ll find several tavernas on the water’s edge and a flock of sea geese eager to sample your leftovers.
During Tihar, on successive days, crows, dogs, and cows are honored by giving them treats to eat and garlands to wear. (Cats, by the way, are considered unlucky and are rarely seen in Nepal.) On the fifth day, brothers are honored by their sisters, who deck them with flowers, place the tika dot on their forehead, and tie a good-luck thread around their left wrists.
At the summit is one of the oldest stupas in the world, an immense white mound surmounted by a golden cube, on the four sides of which are the astonishing all-seeing eyes of Buddha. Above this rises a tower of 13 diminishing golden disks symbolizing the 13 steps to enlightenment, then a golden royal parasol topped by a bell-shaped crown. Strings of prayer flags stretch from the tower’s pinnacle, and around the base are hundreds of small prayer wheels. While pilgrims circumambulate the stupa, monkeys, dogs, and pigeons clamber about and forage for scraps of food offerings in small altars set in the foundation.`
Within all the files, this command displays all the lines in each text file that contains the string "dog". In this case, since "dog" is a common word, hence why we see so many lines. We print all the lines so the output is long.
Here is another use but in another file.

input: `grep -h "dog" berlitz1/*.txt`

output:
`across Gaul, controlling Langue­doc, Dordogne, and a large part of
        Inland from the Atlantic coast — Aquitaine, Dordogne,
        Favorite Lake District competitions range from wrestling and sheep dog
        deer, so-called because it bays like a dog when threatened by
        wreaks havoc with the unwary, and it really is a case of “only mad dogs
        and Englishmen,” as Noel Coward put it. Leave it to the mad dogs. Half
        dogs, and goats breathing the fumes of hundreds of buses and cars.
        Sheepdog trials
        The way sheepdogs do their job is a source of fascination
        summer local farmers and their dogs get together for a friendly
        competition; the dog and farmer maneuver sheep around a set course.
        aniseed-scented trail is laid on the morning of the race, and the dogs
        not think so when the dogs reappear and the enthusiastic owners call,
        grabbing a hot dog and a beer and rooting for the Dodgers baseball team
        flowers gently held in the mouths of some very patient-looking dogs is
        Walter Scott (and his faithful dog, Maida) carved from Cararra marble.
        Cister­cian order, you’ll notice a niche for a guard dog below the
        626 char­ac­ters, 202 horses, 55 dogs, and 505 other animals.
        In and around the lovely valley of the Dordogne, Périgord
        Many visitors driving from Paris to the Dordogne and
        out to the Atlantic Ocean. Of these, the Dordogne has carved a
        four teenagers chasing a dog in 1940.
        Dordogne
        The name Dordogne is given to a river, a département of
        Start at the confluence of the Vézère and Dordogne rivers,
        At the western end of the Dordogne Valley, this is
        watching the sunset, dogs and cats underfoot, songbirds in bamboo cages
        chickens, you will see for sale snakes, dogs, bats, and sometimes
        may splash you; children, dogs, and cats may get in your way; and the
        far from Bagdogra. Built in 1881, the tiny steam-train on a 60-cm
        Campidoglio (Capitoline Hill). This quiet traffic-free haven forges a
        Campidoglio (see page 50), have extensive collections of sculpture
        is the Porta della Carta (Gate of the Paper, where the doge posted his
        decrees and scribes gathered). The Gothic sculpture shows the doge
        their secret deliberations. The last doge presented his abdication to
        Napoleon here. Of the 76 doges portrayed here, one is blackened out,
        adorns the entrance wall above the doge’s throne. Said to be the
        wander around the lobby of the venerable Danieli Hotel, a former doge’s
        Guggenheim and her dogs are buried here. A lovely limited-menu café
        Built by the Dominicans, it was the doges’ funeral church with some 25
        Pisani doges in 1756, with 200 rooms, Tiepolo frescoes in the ballroom,
        commuting Nichiren’s sentence to exile on the island of Sadogashima.
        playgrounds for the children. Special events such as pet shows, dog
        sheep. They also regularly hold sheep dog and sheep-shearing
        Elsewhere, there are miniature palheiro dog kennels, and`

<h2>I will use 'grep -v'</h2>

input: `grep -v "the" WhatToLasVegas.txt`

output: 
 `What To Do
        To say that Las Vegas is a non-traditional city barely
        begins to hint at what a trip here will foretell. To say that gambling
        industry.
        metropolis of over one million residents whose primary industry is
        “what to do” and “where to go” difficult to delineate. In Las Vegas,
        interdependent.
        Until relatively recently, entertainment industries in Las
        traditional, off-Strip experiences, thus sparking a growth in local
        culture and amenities. Today, that process is still young but steadily
        independent cultural amenities found in a more traditional city of its
        unexpected.
        Gambling
        Since 1931, when gambling was officially legalized in Nevada
        that one can legally place bets on games of chance and sporting events.
        would be no Forum Shops, no pirate ships, no Bellagio Gallery of Fine
        Art.
        Strip, where nearly twenty major casinos in excess of 100,000 sq ft
        One. ”
        furious, with generally inflexible house rules. Downtown casinos are a
        bit more flexible when it comes to house rules, offering lower minimums
        combination of serious career gamblers and novices without much to
        to a small town — one that has not changed much in 70 years.
        It is important to keep in mind that before you venture
        to overcome your lack of knowledge. The first would be to read about
        many books are sold locally that go to great lengths to explain each
        game.
        wagers as low as 5¢ and a distinct lack of potentially impatient
        players waiting for you to decide your next move, electronic gaming is
        an alternative that many novice gamblers never move beyond. Most
        casinos offer a variety of video game slot machines. Try Bally’s for
        gaming, it makes little sense to spend your vacation in Las Vegas and
        not play at least a few hands of blackjack or craps, especially when
        lessons are taught by dealers to groups of novices, so no one feels
        learn a game and its rules without risking your money or your
        pride.
        Baccarat
        Typically assumed to be a high-roller card game, baccarat
        (bah-cah-rah) is similar to blackjack, though it’s played with stricter
        dealer). Most baccarat tables are located in quiet, sequestered
        this game.
        Big 6 (or Money Wheel)
        This spin-and-win (or more often lose) game looks strangely
        Bingo
        in which players try to line up a horizontal or vertical row of
        randomly drawn numbers. The numbers are drawn until someone wins, and
        some veterans get up to 10 cards playing at once. No lessons are
        required.
        Black Jack (or 21)
        close to 21 as possible without “busting” (going over 21). There are
        several optional bets — splitting, doubling down, insurance — and
        variations that include single-deck vs. multi-deck card shoes and hands
        dealt face-up (as opposed to one card down). The house advantage is
        well.
        Craps
        candidate for lessons. Don’t even lean against a busy craps table
        unless you know what you’re doing and have plenty of money to lose.
        Keno
        odds are shifted in that players circle random numbers on a purchased
        ticket and wait for a fixed set of numbers to be drawn. It’s easy to
        you to see if enough of your numbers come up to win. The odds of
        time while you’re dining.
        Poker
        A high-stakes card game played in a high-pressure
        you. ” )
        Pai Gow
        If you enjoy poker, playing at mild pace, and playing
        against no house advantage, you’ll love Pai Gow. Each player is dealt
        five-card hand and one two-card hand. Standard poker rules apply; that
        is, pairs, straights, flushes, full houses, etc. are ranked in a
        “push” (tie), and no money changes hands (this happens more often than
        advantage, it takes 5% of your winnings.
        Roulette
        enjoy much popularity in Las Vegas. It’s a relatively simple game,
        where bets are placed by laying chips on a single number or groups of
        numbers, colors, or odd/even. Different players are given different
        avoid playing a double-zero wheel and search for those with only one
        zero. ) Winning numbers are illuminated at each table to attract
        passers-by into thinking “It’s hitting my number! ”
        Slots
        computer that’s programmed to pay out big money. But what do you think
        Video Poker
        Video poker has become increasingly popular, so much so
        slots, interaction and a semblance of skill are required; that is, you
        The Big Shows
        Once, Las Vegas showrooms were filled with top
        entertainment — headliners, comedians, production shows, and dancing
        girls — that could be enjoyed at a very low price. In that bygone era,
        elaborate dinner shows were considered a loss leader, a way to keep
        entertainment and food.
        When corporations moved in with more stringent departmental
        accounting procedures, every sector of a hotel-casino had to show
        success. Not satisfied with a simple overall profit, corporate
        operators began to both raise prices and cut corners, resulting in an
        era of frustrating mediocrity from which Las Vegas has only recently
        emerged.
        Most showrooms are again offering quality stars and
        bigger shows and headliner appearances (especially during major events
        like New Year’s Eve) exceed $100 per ticket — typical for New York
        City, but previously unheard of in Las Vegas. What this means is that,
        pay for now applies equally to Las Vegas.
        open-ended, remember that nothing is static in Las Vegas. Entire
        resorts open and close, and showrooms sometimes change show times,
        headlining entertainers that change from week to week. For current
        listings of all resort entertainment, pick up a free copy of Showbiz
        all. Be advised that it is traditional for showgirls in Las Vegas
        production shows to be topless, and that tradition continues; many
        shows are not appropriate for children.
        performers provide energetic renditions of Madonna, Michael Jackson,
        Girls impersonators still have Ginger. Stratosphere Hotel and Casino,
        2000 Las Vegas Boulevard South; Tel. (702) 380-7777. Shows 7 and 10pm,
        no late show Sunday–Tuesday; dark Thursday; $38 or less (special rate
        for children 4–12).
        Caesars Magical Empire: A particularly unusual interactive
        Casino, 3570 Las Vegas Boulevard South; Tel. (702) 731-7110. Multiple
        seatings start at 5pm; dark Sunday and Monday; around $75 (special rate
        for children 5–10).
        Cirque du Soleil’s Mystère: The internationally famed
        performers of amazing physical and emotive skill and grace. A most
        unique Las Vegas experience that borders on performance art. This
        3300 Las Vegas Boulevard South; Tel. (702) 894-7111. Shows 7:30 and
        10:30pm; dark Monday and Tuesday; over $60.
        international troupe, O dazzles in an aquatic environment that utilizes
        Hotel and Casino, 3600 Las Vegas Boulevard South; Tel. (702) 693-7111.
        Shows 7:30 and 11pm; dark Wednesday and Thursday; over $100.
        Danny Gans – The Man of Many Voices: What started as a
        entertainment. Mirage Hotel and Casino, 7900 Las Vegas Boulevard South;
        Tel. (702) 791-7111. Shows 8pm; dark Monday and Frida y; over $60.
        EFX: A grand $45 million production show in a classic but
        talents, EFX is a special-effects laden science-fiction tale suitable
        for all ages. MGM Grand Hotel and Casino, 3799 Las Vegas Boulevard
        South; Tel. (702) 891-7777. Shows 7:30 and 10:30pm; dark Sunday and
        Monday; over $50.
        Wayne Newton: Las Vegas’s copnsummate entertainer, Wayne
        Newton croons to audiences six nights a week in an elaborate new
        Las Vegas Boulevard South; Tel. (702) 732-6111. Shows 9pm
        Sunday–Thursday; 8 and 11pm Saturday; dark Friday; $60 or less.
        Blue Man Group: This award-winning (albeit unusual) show
        features three bald, blue characters. The one-of-a-kind showroom
        experience has been called innovative, hilarious, and musically
        powerful. Luxor Hotel and Casino, 3900 Las Vegas Boulevard South; Tel.
        (702) 262-4100. Shows 7 and 10pm (no late show Sunday and Monday); dark
        Tuesday; over $50.
        amazing special effect. The show also features magician Dirk Arthur and
        dozens of topless and costumed showgirls, making this an event for
        adults only. Bally’s Hotel and Casino, 3645 Las Vegas Boulevard South;
        Tel. (702) 967-4111. Shows 7:30 and 10:30pm Wednesday–Monday; dark
        Tuesday; $45–60.
        King Arthur’s Tournament: A radical departure from modern
        Las Vegas stage shows, this one features two unusual elements: live
        re-creation of a medieval knights’ jousting tournament, it’s great fun
        for families. Excalibur Hotel and Casino, 3850 Las Vegas Boulevard
        South; Tel. (702) 597-7777. Shows 6 and 8:30pm; $45 or less.
        Legends In Concert: The favorite of many return visitors,
        Four Tops and Elvis, as well as modern stars like Michael Jackson and
        Tina Turner. Imperial Palace Hotel and Casino, 3535 Las Vegas Boulevard
        South; Tel. (702) 731-3311. Shows 7:30 and 10:30pm; dark Sunday; $35 or
        less.
        that somehow maintains intimacy — magician Lance Burton pulls off
        dancers. Monte Carlo Hotel and Casino, 3770 Las Vegas Boulevard South;
        Tel. (702) 730-7777. Shows 7 and 10pm; dark Sunday and Monday; $60 or
        less.
        choreographer of Riverdance comes this Las Vegas production, an
        internationally recognized hit featuring over 40 talented dancers in an
        amazing show of traditional and modern dance. New York-New York Hotel
        and Casino, 3790 Las Vegas Boulevard South; Tel. (702) 740-6969. Shows
        7:30 and 10:30pm Tuesday, Wednesday, Saturday; 9pm Thursday and Friday;
        dark Sunday and Monday; $50–80.
        Siegfried and Roy: These world-famous illusionists and Las
        Vegas residents have risen from a small-time specialty act to stardom.
        1500-seat showroom. Mirage Hotel and Casino, 3400 Las Vegas Boulevard
        South; Tel. (702) 791-7444. Shows 7:30 and 11pm; dark Wednesday and
        Thursday; over $60.
        production shows, Splash features a large cast of singers and dancers
        Casino, 2901 Las Vegas Boulevard South; Tel. (702) 734-5110. Shows 7:30
        and 10:30pm; $36–60.
        Tropicana’s show was recently revamped and updated. Nothing says “Las
        3801 Las Vegas Boulevard South; Tel. (702) 739-2222. Shows 7:30 and
        10pm; dark Thursday; $40–60.
        Shopping
        seem. As with everything else in Las Vegas, shopping facilities have
        not live up to expectation. Hotel shopping areas consisted of retailers
        selling primarily expensive and tacky (or sometimes cheap and tacky)
        merchandise, and malls were utilitarian outlets of typical retail
        stores. This scenario has changed dramatically in recent years.
        department stores have arrived at suburban malls in recent years,
        name designers now have retail locations in several hotel shopping
        resorts.
        drive, and a handful of local shops that deserve attention.
        Retail Shopping Malls
        indoor shopping promenade built to look and feel like an outdoor Roman
        street, surprised quite a few observers in 1992 by attracting not only
        location here. The number of excellent restaurants and entertainment
        outlets makes this a great place for an all-day, one-stop spending
        spree.
        tourists and residents with excess cash. Though it has since been
        department stores, as well as a huge food court.
        is not.
        Factory Outlet Malls
        The Fashion Outlet Mall (Tel. 702/874-1400) at Primm,
        (Guess, Kenneth Cole, Tommy Hilfiger) and specialty stores (such as
        702/896-5599). Belz, an indoor mall, offers 145 stores ranging from
        clothing to electronics.
        Selected Local Shopping
        From ethnic food shops and vintage clothing stores to electronics and
        Vegas highlights; for a more thorough listing of specialty stores, pick
        Weekly.
        vintage store in America, owing to its feature in both a Visa
        commercial and on extreme sports network ESPN II. A massive two-story
        serves an international audience with its wide selection of period
        clothing. They are often called upon to provide items for movies being
        filmed in Las Vegas.
        Superstore (Tel. 702/364-2500) sells nothing even remotely vintage,
        except perhaps within its vast CD selection. A combined effort of Tower
        innumerable aisles of records, books, software, CDs, 12-inch vinyl, and
        is a coffee bar and café under a giant screen television flanked by CD
        listening stations.
        of Optica of Las Vegas (Tel. 702/735-8557), a full service optometry
        shop that can repair eyewear, provide exams, and set visitors up with a
        new set of prescription glasses or contact lenses — all within a day or
        Gamblers’ General Store (Tel. 702/382-9903), a centrally located
        request.
        Smoke Shop (Tel. 702/387-6433) sells tax-free tobacco products through
        spend all that money you just saved.
        Sports
        and/or plenty of cash. If you engage in outdoor sports, remember that
        valley temperatures can reach well above 100º F (38º C) in summer and
        all necessary precautions when participating in any outdoor sport.
        Spectator Sports
        Boxing
        Las Vegas has a rich boxing history, having hosted enough
        MGM Grand (Tel. 702/891-7777), Caesars Palace (Tel. 702/731-7110), or
        The Mirage (Tel. 702/791-7111) — invariably draws a crowd heavy with
        celebrities.
        The National Finals Rodeo
        nation’s top cowboys and cowgirls riding bulls, busting broncos, and
        endless satellite events: beauty pageants, parties and dances at bars,
        Experience, and golf tournaments. If you wish to attend, plan
        by.
        Motor Sports
        Downtown on Interstate 15. The 1,500-acre (607-hectare) site is a
        speed-freak’s dream: a 11⁄2-mile (21⁄2-km) tri-oval super speedway,
        smaller clay and paved ovals, a drag strip, a road track, and a
        Golf Tournaments
        The Las Vegas Invitational held every fall — famed as Tiger
        <www.pgatour.com> for complete information on tournaments and on
        Bowling
        Las Vegas has always had an affinity for bowling. The PBA
        Showboat Bowling Center in January.
        Las Vegas, while lacking a major sports franchise, is home
        to a triple-A baseball team and a minor-league hockey squad. The Las
        outfit — is a farm team for baseball’s San Diego Padres;tickets are
        Thunder hockey team (which is not affiliated with any NHL franchise)
        title in 1990.
        Participatory Sports
        Golf
        For a desert city, Las Vegas has more than enough grass
        locator map and a course-by-course description, go to
        <www.lasvegasfreedom.com>. The Rio Suites Hotel maintains a
        702/254-4653) is a municipal course with a difference: it has two
        18-hole courses designed by Arnold Palmer and a 12-hole par-3 course
        Vegas Paiute Resort (Tel. 702/658-1400) is 20 miles (32 km) north of
        Rock Climbing
        Red Rock Canyon (Tel. 702/363-1921), just 20 minutes from
        States. There are literally thousands of climbing challenges, from
        small bouldering routes to towering, experts-only cliffs. Spring and
        fall are optimum climbing seasons, but almost any weekend will find a
        climbing trips of nearly any duration. For a more climate-controlled
        highest.
        Hiking
        The Las Vegas Valley is rimmed with quality hiking trails.
        Vegas Valley. Red Rock Canyon affords numerous routes, including a
        Keystone Thrust Trail. Likewise, Mount Charleston is webbed wit h many
        (702/873-8800). Valley of Fire (see page 66) is also a popular hiking
        spot.
        Bicycling
        busier streets; bike paths are few and courteous drivers even fewer.
        The best places are local parks or bike-friendly spots beyond city
        picturesque landscapes and is not overly taxing. Mountain bikers can
        Floyd Lamb State Park (702/486-5413), a few miles north on US 95. The
        bike paths wind among ponds, trees, and historic buildings.
        Tennis
        Most resorts have tennis facilities for guests only.
        membership sporting club, makes its courts available to nonmembers as
        well, and several additional courts can be found in Lorenzi Park.
        Snow Sports
        Snowboard Resort, also known as Lee Canyon (Tel. 702/872-5462). It has
        ski rental, ski school, and a lounge. The natural snowfall is often
        augmented by snow-making equipment to ensure adequate powder. The Las
        Vegas Ski and Snowboard Resort has nine long runs on 40 acres (16
        hectares); despite its name, snowboarding is allowed only at certain
        times.
        Adult Entertainment
        its existence as a tourist city.
        during convention season.
        Avenue (Tel. 702/384-0074), an intimate, friendly place, and Olympic
        Garden Cabaret, 1531 Las Vegas Boulevard South (Tel. 702/385-8987)
        venerable Palomino Club, 1848 Las Vegas Boulevard North (Tel.
        3340 S. Highland Drive; Tel. (702) 796-3600.
        Nightlife
        answer is a resounding yes. From local bars featuring live music and
        beyond gambling and shows is very healthy. For a detailed listing of
        newsweeklies, CityLife or Las Vegas Weekly.
        Nightclubbing has come of age in Las Vegas, thanks to a
        Suites Hotel, led to a deluge of new hotel-based high energy clubs,
        Grand (Tel. 702/891-1111), and more scheduled to open soon. Each caters
        you.
        dancing, including Drink Las Vegas (Tel. 702/796-5519), a fabulous
        two-story nightclub with numerous bars serving every drink known to
        man. The Beach (Tel. 702/731-1925) is also two stories high, with
        bar for a little bikini dancing.
        Lesbian and gay travelers will find integrated nightlife
        702/731-1919) is small but wall-to-wall with energetic dancing (it’s
        bar.
        The café scene is surprisingly strong for a city with so
        many Starbucks outlets. Café Copioh (Tel. 702/739-0305) is a well known
        haunt of university students and professors, and hosts a calendar of
        its Bohemian glory.
        702/386-0999). Lawyers, poets, city councilmen, and starving musicians
        partake day and night of its garden setting and large menu featuring
        direction you’ll enjoy Jazzed Cafe and Vinoteca (Tel. 702/798-5995), a
        carefully crafted menu of Tuscan specialties accompanied by acid jazz,
        tiramisù and espresso. Best of all, it’s open until about 4am.
        Las Vegas for Children
        are a surprising number of kid-friendly activities. Most casinos have
        m) of games (more than 250) from traditional pin-ball outposts to
        high-tech diversions. If you play up an appetite, GameWorks also has a
        full-service restaurant, snack bar, and Starbucks Coffee outlet. Adults
        Add a little zoom to your kids’ day with a stop at Sahara
        Speedworld (Tel. 702/737-2111), a huge (40,000-sq-ft /3720-sq-m)
        playground of virtual reality auto racing in life-size race cars,
        Visitors between May and September can take tots and teens
        There are kiddie pools and knee-buckling water slides. Der Stuka offers
        In recent years, as it sought to attract more families,
        and summer only), visitors can raft a small river, take a 200-ft (61-m)
        with strolling MGM characters.
        with Grand Slam Canyon (Tel. 702/734-0410), a pink-dome-covered,
        roller coaster, a water ride, bumper cars, carnival games, and a laser
        features kid-friendly free circus acts from 11am to midnight daily.
        twisting, turning, looping Manhattan Express roller coaster at New
        doesn’t melt in your hand. Inside is an 8,500-sq-ft (791-sq-m) store
        loaded with thousands of M&M knickknacks.
        three-course miniature golf, bumper boats, go-carts and arcade games at
        Scandia Family Fun Center (Tel. 702/364-0070).
        (Tel. 702/875-4191), a mock ghost town near Red Rock Canyon. The
        wild-West town comes complete with gunfights, a wax museum, an opera
        house, a mini-train, horseback riding, and an extensive petting
        zoo.
        For motorized thrills, Las Vegas has at least one grand
        prix go-cart course. Las Vegas Mini Gran Prix (Tel. 702/259-7000)
        (3-hectare) facility has wheels for adults as well.
        For something a little more aggressive, Desert Storm
        warriors — over age 10, that is.
        Local Arts
        Although Las Vegas isn’t known for its culture, that
        Vegas also constitute a center of cultural activity. The Summerlin
        Library and Performing Arts Center (Tel. 702/256-5111) features an art
        Nevada Arts Council (Tel. 702/486-3700).
`
For this command, it compiles all the lines that don't have the string "the". I made sure to pick a common word.
Otherwise, this would be very large. I also focused on what text file to search the string.

input: `grep -v "the" IntroIbiza.txt`

output: 
`•Ibiza and Formentera
        of neighbouring Mallorca and Menorca, with which it is commonly
        fray.
        •Formentera, Ibiza’s diminutive neighbour just one hour’s
        apart — in some ways more like a desert island than a satellite or
        exuberant nightlife back on “mainland” Ibiza. Alternatively, if you
        Ibiza are dotted with a host of minor islets, most uninhabited but all
        eminently explorable.
        •One thing you’ll quickly realize about Ibiza is its
        laissez-faire attitude towards life. On this island paradise, tourists
        one of those barren Mediterranean rocks with an allure that begins and
        usual bullfight-and-flamenco scene. The people are a distinct race:
        though Castilian is spoken as well.
        Catalonian city of Barcelona. With an area of just 541 sq km (209 sq
        but it is big enough to contain a modest mountain, verdant farms,
        highest peak, Mount Sa Talaia, or Atalaya (475 meters/1,558 feet),
        •The climate here is distinctly Mediterranean: temperature
        •The capital of Ibiza, called simply Ibiza, or Ibiza Town,
        financial, governmental, and administrative centre, and its charms
        popularity is such that it has gained a reputation for being something
        to be.
        Antoni Abad (San Antonio in Castilian or Abbot St. Anthony in English).
        Janeiro’s Copacabana Beach, are high-rise hotels and apartment
        buildings. The resort is a centre not only for beach activities but for
        lively nightlife as well.
        this was merely a hamlet on a hilltop crowned by a picturesque
        by.`
Luckiliy in this case, "the" was very common. Hence the shorter output.

<h2>I will use 'grep -w'</h2>
Brief Introduction: This command is used especially for finding substrings as it will return the line that contains that substring
no matter if it is an actually a word or not. This would be most appropiate for finding prefixes or suffixes.

input:
`grep -w "re" IntroIbiza.txt`

output:
`almond trees are objects of beauty and colour; for the farmer, they’re`

This command is useful when you want to find a prefix or certain substring, regardless if its connected to another word.

I will try with another substring that's unique

input:
`grep -w "hat" IntroIbiza.txt`

ouput:

There was no output. There didn't even contain the word "that" which would trigger this command to spit out the line it is in.


<h1>Source</h1>
[Source_Geeks_for_Geeks](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)

        

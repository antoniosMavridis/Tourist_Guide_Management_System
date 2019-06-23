
destination_type(mountainous).
destination_type(island).
destination_type(coastal).

sights_type(museums).
sights_type(sports).
sights_type(tour).

accommondation(hotel).
accommondation(motel).
accommondation(studio).

room_type(single).
room_type(double).
room_type(triple).

cost(300).
cost(700).
cost(1500).

transportation(bus).
transportation(airplane).
transportation(boat).


destination(pelion,mountainous,bus,museums,hotel,single,300).
destination(pelion,mountainous,bus,sports,motel,double,700).
destination(pelion,mountainous,bus,museums,hotel,triple,300).
destination(karpenisi,mountainous,bus,museums,hotel,single,700).
destination(karpenisi,mountainous,bus,museums,hotel,double,1500).
destination(karpenisi,mountainous,bus,tour,motel,triple,700).

destination(santorini,island,boat,sports,hotel,single,700).
destination(santorini,island,boat,tour,studio,double,700).
destination(santorini,island,airplane,sports,hotel,double,1500).
destination(rhodes,island,boat,sports,hotel,single,700).
destination(rhodes,island,airplane,museums,motel,triple,1500).
destination(rhodes,island,boat,tour,studio,single,300).

destination(nafplio,coastal,bus,sports,hotel,single,300).
destination(nafplio,coastal,bus,museums,hotel,double,700).
destination(nafplio,coastal,bus,tour,hotel,triple,1500).
destination(chalkidiki,coastal,bus,sports,hotel,triple,1500).
destination(chalkidiki,coastal,airplane,museums,studio,double,1500).
destination(chalkidiki,coastal,airplane,tour,motel,single,700).

details(pelion,"Sights: Portaria","Routes:Athens-Volos-Pelion","Services: Hospital").
details(pelion,"Sights: Church of Taxiarches","Routes:Thessaloniki-Larisa-Pelion","Services: Hospital").
details(karpenisi,'Sights: Ski-center','Routes:Athens-Volos-Karpenisi','Services: Super market').
details(karpenisi,'Sights: Holy Trinity Metropolitan Church','Routes:Pireaus-Volos-Karpenisi','Services: Super market').

details(santorini,"Sights: Volcano","Routes:Athens-Crete-Santorini","Services: police,tourist office").
details(santorini,"Sights: Red sea","Routes:Athens-Mykonos-Santorini","Services: police,tourisτ office").
details(rhodes,"Sights: Knight Castle","Routes:Athens-Crete-Rhodes","Services: Super market").
details(rhodes,"Sights: surfing","Routes:Athens-Skopelos-Rhodes","Services: pharmacy").

details(nafplio,"Sights: Castle","Routes:Athens-Pireaus-Nafplio","Services: Super market").
details(nafplio,"Sights: Archaelogical museum","Routes:Athens-Pyrgos-Nafplio","Services: police").
details(chalkidiki,"Sights: Sea","Routes:Athens-Larisa-Chalkidiki","Services: tourisτ office").
details(chalkidiki,"Sights: Byzantine museums","Routes:Athens-Volos-Chalkidiki","Services: Hospital").




tourist_office:-         write("Enter the type of destination type(mountainous,island,coastal):"),
                         nl,
                         read(A),
                         write("Enter the type of sights(museums,sports,tour):"),
                         nl,
                         read(B),
                         write("Enter the type of accommondation(hotel,motel,studio):"),
                         nl,
                         read(C),
                         write("Enter the type of rooms(single,double,triple):"),
                         nl,
                         read(D),
                         write("Enter the maximum cost($):"),
                         nl,
                         read(E),
                         write("Enter the type of transportation(bus,airplane,boat):"),
                         nl,
                         read(F),
                         assertz(destination_type(A)),
                         assertz(sights_type(B)),
                         assertz(accommondation(C)),
                         assertz(room_type(D)),
                         assertz(cost(E)),
                         assertz(transportation(F)),

                         destination(L,A,F,B,C,D,E),
                         details(L,W,Y,T),


                         write("The best destination for you is: "),write(L),nl,
                         write("Some details for the destination:"),nl,
                         write(W),nl,
                         write(Y),nl,
                         write(T),nl.

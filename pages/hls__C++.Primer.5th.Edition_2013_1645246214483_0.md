file-path:: ../assets/C++.Primer.5th.Edition_2013_1645246214483_0.pdf
file:: [C++.Primer.5th.Edition_2013_1645246214483_0.pdf](../assets/C++.Primer.5th.Edition_2013_1645246214483_0.pdf)
title:: hls__C++.Primer.5th.Edition_2013_1645246214483_0

- e base class definesasvirtualthose functions it expects its derived classes to define for themselves.
  ls-type:: annotation
  hl-page:: 621
  id:: 62107946-c1ee-4a85-a5d2-dabff6ede9df
- dynamic  binding  happens  when  a  virtual  function  is  calledthrough a reference (or a pointer) to a base class.
  ls-type:: annotation
  hl-page:: 623
  id:: 62107a86-3ce4-424e-a578-4496c31bef0d
- a base class must distinguish the functions it expects its derived classesto override from those that it expects its derived classes to inherit without change.
  ls-type:: annotation
  hl-page:: 624
  id:: 62107d60-f689-4eb5-b732-a73fe1322f8b
- When we call a virtual functionthrough a pointer or reference, the call willbe dynamically bound. Depending on the type of the object to which the referenceor pointer is bound, the version in the base class or in one of its derived classes willbe executed.
  ls-type:: annotation
  hl-page:: 624
  id:: 62107e0a-3dac-434b-b0dc-638e48db8dbc
- [:span]
  ls-type:: annotation
  hl-page:: 626
  id:: 621096de-f71c-4a2d-8014-7ee663dfe6df
  hl-type:: area
  hl-stamp:: 1645254365423
- [:span]
  ls-type:: annotation
  hl-page:: 626
  id:: 621097cb-c852-427b-950c-e60e5dee54b1
  hl-type:: area
  hl-stamp:: 1645254602517
- a derived class must use a base-class constructor to initialize itsbase-class part.
  ls-type:: annotation
  hl-page:: 627
  id:: 621098a4-0851-414f-b24c-30542cdde628
- The base class is initialized first, and then the members of the derivedclass are initialized in the order in which they are declared in the class.
  ls-type:: annotation
  hl-page:: 627
  id:: 6210996f-7bd1-4e17-9954-e2df3be88587
- A derived class may access thepublicandprotectedmembers of its base class
  ls-type:: annotation
  hl-page:: 627
  id:: 6210998f-2c4b-4255-b0b2-1167e1cfabf5
- Interactions withan object of a class-type should use the interface of that class, even if that object is thebase-class part of a derived object.
  ls-type:: annotation
  hl-page:: 628
  id:: 62109a36-df8c-4a38-9d53-d2c6bd6af546
- [:span]
  ls-type:: annotation
  hl-page:: 628
  id:: 62109b41-8a35-427a-913f-ba265b8c0713
  hl-type:: area
  hl-stamp:: 1645255488715
- :  We can bind a pointer or ref-erence to a base-class type to an object of a type derived from that base cl
  ls-type:: annotation
  hl-page:: 630
  id:: 6210d17f-6a3b-4aad-a2b6-b7065fb346a9
- e static type of an expression is always known atcompile time
  ls-type:: annotation
  hl-page:: 630
  id:: 6210d24a-29b8-4312-b506-814eb92841ae
- dynamic type is the type of the object in memory that the variable orexpression represents
  ls-type:: annotation
  hl-page:: 630
  id:: 6210d262-85ef-487d-9455-7e8cd5f74e47
- The dynamic type of an expression that is neither a reference nor a pointer isalways the same as that expression’s static ty
  ls-type:: annotation
  hl-page:: 631
  id:: 6210d552-e84f-4806-8183-db522035854e
- The conversion from derived to base existsbecause every derived object contains abase-class part to which a pointer or reference of the base-class type can be bou
  ls-type:: annotation
  hl-page:: 631
  id:: 6210d58b-6747-483f-af10-a1e4145c9f0d
- [:span]
  ls-type:: annotation
  hl-page:: 631
  id:: 6210d5fe-2d6f-4df0-a752-9bbb38a94da4
  hl-type:: area
  hl-stamp:: 1645270524571
- t we cannot convert from base to de-rived even when a base pointer or reference is bound to a derived ob
  ls-type:: annotation
  hl-page:: 631
  id:: 6210d78f-a858-4f4b-ae8a-fb881177e1bf
- in C++dynamic binding happens when a virtual member functionis called through a reference or a pointer to a base-class type 
  ls-type:: annotation
  hl-page:: 632
  id:: 6210eb6b-c696-4e32-b4f8-a45c1ef514ee
- [:span]
  ls-type:: annotation
  hl-page:: 633
  id:: 6210ef94-4f86-4314-9aa7-d3db3def0f62
  hl-type:: area
  hl-stamp:: 1645277075237
- [:span]
  ls-type:: annotation
  hl-page:: 634
  id:: 6210f1dd-0bb7-4b78-a042-56163c3d4928
  hl-type:: area
  hl-stamp:: 1645277660083
- A derived-class function that overrides an inherited virtual function must haveexactly the same parameter type(s) as the base-class function that it overri
  ls-type:: annotation
  hl-page:: 634
  id:: 6211096f-5610-4525-b61f-033bda92cce7
- [:span]
  ls-type:: annotation
  hl-page:: 636
  id:: 6211177d-a219-4011-af4a-74851783fd69
  hl-type:: area
  hl-stamp:: 1645287291841
- A class containing (or inheriting without overridding) a pure virtual function isanabstract base class
  ls-type:: annotation
  hl-page:: 639
  id:: 6211212c-f453-4af8-a847-13cb26f51a7c
- Access to a member that a class inherits is controlled by a combination of the accessspecifier for that member in the base class, and the access specifier in the derivationlist of the derived clas
  ls-type:: annotation
  hl-page:: 641
  id:: 6211dc45-5326-40be-976e-7471cdb5b737
- The derivation access specifier has no effect on whether members (and friends) ofa derived class may access the members ofits own direct base class
  ls-type:: annotation
  hl-page:: 641
  id:: 6211dd2c-2672-4bea-addb-be3132ee55ab
- The purpose of the derivation access specifier is to control the access thatusersof the derived clas
  ls-type:: annotation
  hl-page:: 642
  id:: 6211dd40-b238-4655-a006-47c20a471b5d
- [:span]
  ls-type:: annotation
  hl-page:: 643
  id:: 6211e1df-e18b-443d-9ddd-3dedb1171b21
  hl-type:: area
  hl-stamp:: 1645339102616
- If a name is unresolved within the scope of the derivedclass, the enclosing base-class scopes are searched for a definition of that name.
  ls-type:: annotation
  hl-page:: 646
  id:: 62122e7b-bafc-4d6f-b86a-8a38d5b6314c
- [:span]
  ls-type:: annotation
  hl-page:: 648
  id:: 62123b10-a2f9-475d-82b8-23ba21a2d5b5
  hl-type:: area
  hl-stamp:: 1645361935477
- If the base and derived memberstook arguments that differed from one another, there would be no way to call thederived version through a reference or pointer to the base class. 
  ls-type:: annotation
  hl-page:: 649
  id:: 62123e65-55c5-4aa8-849d-e6b7eca30249
- [:span]
  ls-type:: annotation
  hl-page:: 649
  id:: 62123fb1-b098-4018-810a-4fab20cf4e4d
  hl-type:: area
  hl-stamp:: 1645363120158
- [:span]
  ls-type:: annotation
  hl-page:: 649
  id:: 62123fb9-ae37-47e9-a312-1eb3d9ba4a3b
  hl-type:: area
  hl-stamp:: 1645363128366
- [:span]
  ls-type:: annotation
  hl-page:: 650
  id:: 62123ff6-6d93-46b2-8d54-12029cdd17d5
  hl-type:: area
  hl-stamp:: 1645363189945
- A derived class can override zero or  more  instances  of  the  overloadedfunctions it inherits.  If a derived class wants to make all the overloaded versionsavailable through its type, then it must override all of them or none of them
  ls-type:: annotation
  hl-page:: 650
  id:: 6212415b-5de3-4cae-bfce-217e2aa17e64
- Thedestructor needs to be virtual to allow objects in the inheritance hierarchy to bedynamically allocated.
  ls-type:: annotation
  hl-page:: 651
  id:: 62124360-e1da-4e93-ad89-189c6671d477
- the copy and moveconstructors for a derived class mustcopy/move the members of its base part as well as the members in the derived.
  ls-type:: annotation
  hl-page:: 654
  id:: 62124dd5-69f3-44ec-aeef-52627cff1d2b
- If we want copy (or move) the base-class part,we must explicitly use the copy (or move) constructor for the base classin the derived’s constructor initializer list.
  ls-type:: annotation
  hl-page:: 655
  id:: 62125877-e1a5-4a85-b5b5-9d4e2f2bbefa
- the  compiler  treats  the  object  as  if  itstype changes during construction or destruction.
  ls-type:: annotation
  hl-page:: 656
  id:: 62125a6b-67b2-4049-8b67-b3a179cc5405
- If a constructor or destructor calls a virtual, the version that is run is theone corresponding to the type of the constructor or destructor itself.
  ls-type:: annotation
  hl-page:: 657
  id:: 62125aa8-7a99-4cfb-a6a9-f94d88d19f2b
- a derived class can reuse the constructors defined by itsdirect base class. 
  ls-type:: annotation
  hl-page:: 657
  id:: 62125aca-c57b-4da9-a743-05795ebcbb94
- A  class cannotinherit  the  default,  copy,  and  move  constructors. 
  ls-type:: annotation
  hl-page:: 657
  id:: 62125b13-f074-43e5-86b2-2d795bd7dd8e
- for each constructor in the base class, the compilergenerates a constructor in the derived class that has the same parameter list.
  ls-type:: annotation
  hl-page:: 657
  id:: 62125b61-276f-45e9-aa74-bf08881ce58e
- We cannot put objects of types related byinheritance directly into a container, because there is no way to define a containerthat holds elements of differing types.
  ls-type:: annotation
  hl-page:: 659
  id:: 62130831-13c0-4790-bf3b-dc7bee48d610
- When we need a container that holds objects related by inheritance, we typicallydefine the container to hold pointers (preferably smart pointers (§ 12.1, p. 450)) tothe base class.
  ls-type:: annotation
  hl-page:: 659
  id:: 621313a0-68d5-4c09-a630-d06c341485ab
# Reconstructing-Early-African-American-Film-History
This project was created by UCLA students and faculty members  to reconstruct and revive the history of early African-American silent race films.  The interest for this project was sparked by the Johnson Negro Film Collection at UCLA’s Charles E. Young Research Library. The intention behind this project was to address a too seldom-discussed history, through a structure that would be the most effective for academic research.

To read more about this data, see the [project website](http://dhbasecamp.humanities.ucla.edu/afamfilm/).

[![DOI](https://zenodo.org/badge/22873/miriamposner/af-am-film-data.svg)](https://zenodo.org/badge/latestdoi/22873/miriamposner/af-am-film-data)

Data Dictionary
===========

**People**

Field Name       |     Data Type                                |    Description
--- | --- | ---
  LN              |                 Variant Character Field             |         Last name of person
  FN                     |          Variant Character Field            |          First name of person
  Full name          |              Variant Character Field           |           Full name of person
  AKA                   |           Variant Character Field           |           “Also known as”; any nicknames or variant spellings of person’s name
  DOB             |                 Date                      |                   Person’s date of birth
  DOD                       |       Date                      |                   Person’s date of death
  Notes                 |           Variant Character Field        |              Miscellaneous notes on person at hand, such as significance, relations to other persons in data, connections to films in database, etc.
  Attachments          |            File Attachment           |                   Primary source attachments, photos, etc.
  Films (Appeared in)        |      Variant Character Field; Linked Data Field |  Films in the database the person appeared on-screen in
  Films (Directed)        |         Variant Character Field; Linked Data Field |  Films in the database the person directed
  Films (Produced)        |         Variant Character Field; Linked Data Field  | Films in the database the person produced
  Films (Camerawork)        |       Variant Character Field; Linked Data Field  | Films in the database where the person operated the camera
  Source                    |       Variant Character Field; Linked Data Field  | Primary or secondary source the person is mentioned in for this dataset
  Films (Otherwise involved)   |    Variant Character Field; Linked Data Field |  Films in the database ther person had any part of not including acting, directing, producing, or camerawork.
  Productn Comp. assoc. with   |    Variant Character Field; Linked Data Field |  Production companies the person is associated with
  Theatrical Company assoc. with  | Variant Character Field; Linked Data Field  | Theater companies the person is associated with
  Films                      |      Variant Character Field; Linked Data Field  | Films in the database the person is associated with

 

**Films**

Field Name       |     Data Type                                |    Description
--- | --- | ---
  Title               |             Variant Character Field        |              Title of film
  Alternate title            |      Variant Character Field        |              Any variant name the film may have been referred to
  Genre                  |          Variant Character Field           |           Film’s genre
  Primary Source Verification    |  File Attachment                  |            Primary source in which the film was mentioned, such as ads, articles, pictorials, etc.
  Notes                         |   Variant Character Field             |         Miscellaneous notes
  Production Company          |     Variant Character Field             |         Production company the film is associated with
  Production date          |        Date                              |           Date the film was produced; most dates only include year of production, which is defaulted as January 1st
  Distribution date      |          Date                              |           Date the film was distributed; most dates only include year of production, which is defaulted as January 1st
  Length (reels)         |          Number                              |         Number of reels the film is contained in
  Actors                    |       Variant Character Field; Linked Data Field  | Last names of actors associated with the film
  Directors                    |    Variant Character Field; Linked Data Field |  Last names of directors associated with the film
  Producers                  |      Variant Character Field; Linked Data Field |  Last names of producers associated with the film
  Camerawork                  |     Variant Character Field; Linked Data Field  | Last names of camera workers associated with the film
  Attachments             |         File attachment                           |   Primary or secondary sources, photos, etc.
  Source                   |        Variant Character Field; Linked Data Field  | Primary or secondary source where the film was mentioned for this dataset
  Writer                |           Variant Character Field; Linked Data Field  | Last names of writers associated with the film
  Otherwise Involved      |         Variant Character Field; Linked Data Field  | Last names of anyone otherwise associated with the film
  Link to media         |           Hyperlink                         |           Link to view the film
  Distributor               |       Variant Character Field; Linked Data Field |  Distributor associated with the film
  Producers (Full Name)       |     Variant Character Field            |          Full names of producers associated with the film
  Actors (Full Name)          |     Variant Character Field        |              Full names of actors associated with the film
  Directors (Full Name)      |      Variant Character Field        |              Full names of directors associated with the film
  Otherwise Involved (Full Name)  | Variant Character Field            |          Full names of anyone otherwise associated with the film
  Writer (Full Name)        |       Variant Character Field            |          Full names of writers associated with the film

**Companies**

Field Name       |     Data Type                                |    Description
--- | --- | ---
  Name                        |            Variant Character Field       |               Name of theater company, production company, or distribution company
  White or AfAm Owned          |           Variant Character Field            |          If the company was white-owned or African-American-owned
  Date founded          |                  Date                             |            Date the company was founded; most dates only include the year founded, which then defaults to January 1st
  Date closed               |              Date                              |           Date the company was defunct; most dates only include the year founded, which then defaults to January 1st
  Location Founded                    |    Variant Character Field             |         Location of the company; some entries include exact addresses, while others only include the city and state
  Films (Produced)            |            Variant Character Field; Linked Data Field  | Films the company produced
  Source                        |          Variant Character Field; Linked Data Field |  Primary or secondary source in which the company was mentioned for this dataset
  Notes                       |            Variant Character Field              |        Miscellaneous notes
  Attachments                      |       File Attachment                       |       Primary or secondary sources, photos, etc.
  Associated People               |        Variant Character Field; Linked Data Field  | People associated with the company, mentioned in any primary or secondary source for this dataset
  Films (Distributed)              |       Variant Character Field; Linked Data Field |  Films the company distributed
  Actors in Theater Company        |       Variant Character Field; Linked Data Field  | Last names of actors associated with the theater company, if applicable
  Associated People (Full Name)     |      Variant Character Field             |         Full names of anyone associated with the theater company, if applicable
  Actors in Theater Company (Full Name) |  Variant Character Field            |          Full names of actors associated with the theater company, if applicable

**Sources**

  Field Name       |     Data Type                                |    Description
--- | --- | ---
  Title            |     Variant Character Field                 |     Title of source used in this dataset
  Author LN         |    Variant Character Field                  |    Last name of author
  Author FN         |    Variant Character Field                   |   First name of author
  Date of Publication |  Date                                     |    Date the source was published; if the source only includes the year, the date defaults at January 1^st^
  Publisher        |     Variant Character Field                  |    Publisher of source
  Archive           |    Variant Character Field                   |   Archive where the source can be found
  Location in Archive  | Variant Character Field                    |  Location within the Archive in which the source can be found
  Notes             |    Variant Character Field                   |   Miscellaneous notes about the source
  Attachments       |    File Attachment                           |   Any attachment relevant to the source
  Films              |   Variant Character Field; Linked Data Field  | Films which the source is associated with i.e. mentions, discusses, pictures, etc.
  Production Company  |  Variant Character Field; Linked Data Field  | Production companies which the source is associated with i.e. mentions, discusses, pictures, etc.
  People            |    Variant Character Field; Linked Data Field  | People—such as actors, directors, producers, etc.—which the source is associated with i.e. mentions, discusses, pictures, etc.

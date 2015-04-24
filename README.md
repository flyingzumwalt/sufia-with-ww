# Hydra Head with Sufia and Worthwhile

A sample Hydra Head that relies on both Sufia (For GenericFiles and IR Features) and Worthwhile (for CurationConcerns - aka "Works").
This gives you all of Sufia plus the ability to create Works.

**This is a Proof of Concept for figuring out how to get Sufia to support Works.**  It shows that the two code bases can function together.

To actually use them together smoothly, we will have to remove some parts of worthwhile and replace them with code from Sufia.

## Installation

    $ git clone git@github.com:flyingzumwalt/sufia-with-ww.git
    $ cd sufia-with-ww

... install all of the system dependencies listed in the sufia README, then

    $ bundle install
    $ rake db:migrate
    $ rails s

To create a work, visit /concern/generic_works/new

## Testing

    $ rake jetty:clean
    $ rake spec

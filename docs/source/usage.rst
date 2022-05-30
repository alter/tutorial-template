Usage
=====

.. _installation:

Installation
------------

To use Lumache, first install it using pip:

.. code-block:: console

   (.venv) $ pip install lumache

≈

To retrieve a list of random ingredients,
you can use the ``lumache.get_random_ingredients()`` function:

.. autofunction:: lumache.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
will raise an exception.

.. autoexception:: lumache.InvalidKindError

For example:

>>> import lumache
>>> lumache.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']


Java code
------------

.. code-block:: java

   public class Main {

     public static void main(String[] args) {

       int num = 29;
       boolean flag = false;
       for (int i = 2; i <= num / 2; ++i) {
         // condition for nonprime number
         if (num % i == 0) {
           flag = true;
           break;
         }
       }

       if (!flag)
         System.out.println(num + " is a prime number.");
       else
         System.out.println(num + " is not a prime number.");
     }
   }

JS code
------------ 

.. code-block:: javascript

   :caption: prime.js   
   // input from the user
   const min = parseInt(prompt("Enter a min value: "));
   const max = parseInt(prompt("Enter a max value: "));

   // generating a random number
   const a = Math.floor(Math.random() * (max - min + 1)) + min;

   // display a random number
   console.log(`Random value between ${min} and ${max} is ${a}`);
   
   

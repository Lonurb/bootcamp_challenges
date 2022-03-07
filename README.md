 //challenge 1
      public func add(n:Nat, m:Nat): async Nat {
        return(n+m);
      };
 //Challenge 2
      public func square(n:Nat): async Nat {
        return(n*n);
      };
 //Challenge 3
      public func days_to_second(n:Nat): async Nat {
        return(n*24*3600);
      };
  //Challenge 4
      public func increment_counter(n:Nat): async Nat {
        counter+=n
        return(counter);
      };
      public func clear_counter(): async Nat {
        counter:=0
        return(counter);
      };
   //Challenge 5
      public func divide(n:Nat, m:Nat): async Bool {
        if (n%m == 0){
          return(true);
        }
        else {
          return(false);
        };
      };

    //Challenge 6
      public func is_even(n:Nat): async Bool {
        if (n%2 == 0){
          return(true);
        }
        else {
          return(false);
        };
      };
    //Challenge 7
      public func sum_of_array(array:[Nat]): async Nat {
        let sum:Nat=0;
        for (value in array.vals()){
          sum+=value;
        };
        return sum;
      };
    //Challenge 8
      public func maximum(array:[Nat]): async Nat {
        let max:Nat=array[0];
        for (value in array.vals()){
          if (max<value){
            max=value;
          };
        };
        return max

      };
    //Challenge 9
      public func remove_from_array(array:[Nat], n:Nat): async Nat {
        let filtered : List<Nat>
        for (value in array.vals()){
          if (value!= n){
            filtered.append(value);
          };
        };
        return filtered

      };

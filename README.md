
          
            // Add current digit from string b (if exists), otherwise add 0
            if (indexB >= 0) {
                carry += b[indexB] - '0';  // Convert char to int and add to carry
                indexB--;
            }
          
            // Append the current bit (carry % 2) to the result
            result.push_back((carry % 2) + '0');  // Convert int to char and append
          
            // Update carry for next iteration (carry / 2)
            carry /= 2;
        }
      
        // Reverse the result since we built it backwards
        reverse(result.begin(), result.end());
      
        return result;
    }
};

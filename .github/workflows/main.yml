using System.CodeDom.Compiler;
using System.Collections.Generic;
using System.Collections;
using System.ComponentModel;
using System.Diagnostics.CodeAnalysis;
using System.Globalization;
using System.IO;
using System.Linq;
using System.Reflection;
using System.Runtime.Serialization;
using System.Text.RegularExpressions;
using System.Text;
using System;



class Solution
{
    public static void Main(string[] args)
    {
        int N = Convert.ToInt32(Console.ReadLine().Trim());

        Regex regex = new Regex(@"[a-z]{1,20}");
        Regex regex1 = new Regex(@"([a-z]{1,50}@gmail.com)"); 

        List<string> list = new List<string>();

        for (int NItr = 0; NItr < N; NItr++)
        {
            string[] firstMultipleInput = Console.ReadLine().TrimEnd().Split(' ');

            string firstName = firstMultipleInput[0];

            string emailID = firstMultipleInput[1];

            bool name = regex.IsMatch(firstName);
            bool email = regex1.IsMatch(emailID);
            if (name && email)
            {
                list.Add(firstName);
            }
        }
        list.Sort();
        foreach (string item in list)
        {
            Console.WriteLine(item);
        }
        
    }
}

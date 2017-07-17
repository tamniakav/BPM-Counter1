# BPM-Counter1
Just another repository
using System;

namespace BPM_Counter
{
    class Program
    {
        static void Main(string[] args)
        {
            int bpm = int.Parse(Console.ReadLine());
            int beats = int.Parse(Console.ReadLine());           
            
            double bars = beats / 4.00;
            double seconds = 60.00 / bpm;
            seconds *= beats;            
            
            Console.WriteLine($"{Math.Round(bars, 1)} bars - {(int)seconds / 60}m {(int)seconds % 60}s");            
        }
    }
}

# Srf Description
https://www.impossiblesiebel.com/2010/11/quick-genbscript-by-fkirill.html#blog

using System;
using OpenMcdf;
namespace TestMcdf
{
    class Program
    {
        static void Main(string[] args)
        {
            OpenMcdf.CompoundFile cf = new CompoundFile(@"C:\Users\myspa\Videos\Videos\Thumbs.db");
            //cf.RootStorage;
            //cf.RootStorage;
            CFStream cFStream = cf.RootStorage.GetStream("256_513a011ff17be936");
            byte[] bytes = cFStream.GetData();
        }
    }
}

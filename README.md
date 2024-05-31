# 91
// Функція, що повертає вибраний алгоритм
private SymmetricAlgorithm DefineAlg()
{
    if (radioButton1.Checked)
        return new DESCryptoServiceProvider();
    else if (radioButton2.Checked)
        return new TripleDESCryptoServiceProvider();
    else if (radioButton3.Checked)
        return new RijndaelManaged();
    else if (radioButton4.Checked)
        return new RC2CryptoServiceProvider();

    return null;
}

probability distributions part 1

dat = read.csv("femaleMiceWeights.csv")

q1: sum(dat[13:24,2] < mean(dat[1:12,2]))

q2: sum(dat[1:12,2] > mean(dat[13:24,2]))

q3: highfat = s[["hf"]]
    mean(highfat > 30)

population = read.csv("femaleControlsPopulation.csv")

q4:mean(population)

dat = read.csv("femaleMiceWeights.csv")

q5: null = replicate(10000, mean(sample(dat, 12)) - mean(sample(dat, 12)))

    diff = mean(dat[13:24,2]) - mean(dat[1:12,2])

    mean(null > abs(diff))

q6: mean(abs(null) > abs(diff))

# or you can multiply by 2 the value you got from the previous question

    

###############################################
# Write an efficient code that skips a number #
###############################################

# 1
# ISSUE: Resizing vectors is highly expensive and requires redundant memory allocations
# FIX: Initialize a vector
function skip13_unsafe()
    vec = []
    for i in 1:1000000
        if i == 13
            continue
        else
            push!(vec, i)
        end
    end
    return vec # Local scope
end

# 2
# ISSUE: It leaves 13th element uninitialized
# FIX: Use an index to address elemets for value assignment
function skip13_unsafe_2()
    vec = Vector{Int}(undef, 999999)
    for i in 1:1000000
        if i == 13
            continue
        else
            vec[i] = i
        end
    end
    return vec # Local scope
end

# 3
# ISSUE: Performant and flexible but doesn't handle errors
# FIX: Handle errors and notice that max > skip
function skip(min::Int, max::Int, skip::Int)
    index = 1
    vec_size = max - min
    vec = Vector{Int}(undef, vec_size)
    for i in min:max
        if i == 13
            continue
        else
            vec[index] = i
            index += 1
        end
    end
    return vec # Local scope
end

###############################################
###############################################

function check_input()

function skip(min::Int, max::Int, skip::Int)
    if max < skip
        # Throw an error
        println("ERROR: Skip number cannot be smaller than the range maximum value.")
    elseif 
    index = 1
    vec_size = max - min
    vec = Vector{Int}(undef, vec_size)
    for i in min:max
        if i == 13
            continue
        else
            vec[index] = i
            index += 1
        end
    end
    return vec # Local scope
end

    println("ERROR: This fucntion only accepts integer as type.")

# Benchmarking
using BenchmarkTools

begin
println("1. Pusing/resizing a vector of any type:")
@btime skip13_unsafe()
println("2. Altering elements of an initialized vector of Int type:")
@btime skip13_unsafe_2()
end

skip(1, 30, 13)

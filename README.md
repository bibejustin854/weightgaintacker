# weightgaintacker
function calculateWeightGain(initialWeight, finalWeight) {
    /**
     * This function calculates the weight gain between an initial weight and a final weight.
     * 
     * @param {number} initialWeight - The initial weight in kilograms.
     * @param {number} finalWeight - The final weight in kilograms.
     * @returns {number} The weight gain in kilograms.
     */
    
    try {
        // Check if both arguments are numbers
        if (typeof initialWeight !== 'number' || typeof finalWeight !== 'number') {
            throw new TypeError('Both arguments must be numbers');
        }
        
        // Calculate and return the weight gain
        return finalWeight - initialWeight;
    } catch (error) {
        // Log the error
        console.error('Error:', error.message);
        return 0;
    }
}

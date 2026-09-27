This button just communicates to all local menu scripts when to open or closed by using buttons that are tagged with "Button"

example for how other scripts use this module

mainButtonModule.bindableEvent.Event:Connect(function(buttonType)
	if buttonType == "RecipeBook" then
		if recipeMainFrame.Visible then
			closeRecipeBook()
		else
			openRecipeBook()
		end
	else
		closeRecipeBook()
	end
end)

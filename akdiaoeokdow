if whitelistezLOL[game:GetService("RbxAnalyticsService"):GetClientId()] then

                local balloonitem = getItem("hang_glider")

                if balloonitem then

                    local oldfunc = bedwars["HangGliderController"].onEnable

                    bedwars["HangGliderController"].canOpenHangGlider = function() return true end

                    bedwars["HangGliderController"].registerCharacter = function() end

                    pcall(function() bedwars["HangGliderController"].openHangGlider() end)

                    bedwars["HangGliderController"].closeHangGlider = function() end

                    bedwars["HangGliderController"].onDisable = function() end

                    task.spawn(function()

                        task.wait(1)

                        for i, v in pairs(workspace:FindFirstChild("Gliders"):GetChildren()) do

                            if v:IsA("Model") and v.Name == "HangGlider" then

                                v:BreakJoints()

                                for i3, v4 in pairs(v:GetDescendants()) do

                                    if v4:IsA("BasePart") then

                                        v4.CFrame = CFrame.new(0, -1995, 0)

                                    end

                                end

                                v:ClearAllChildren()

                            end

                        end

                    end)

                    bedwars["HangGliderController"].onEnable = function(Self, balloon)

                        local threadidentity = syn and syn.set_thread_identity or setidentity

                        threadidentity(7)

                        task.spawn(function()

                            bypassed1 = true

                        end)

                        threadidentity(2)

                        bedwars["HangGliderController"].onEnable = oldfunc

                    end

                end

                ACDisabler["ToggleButton"](true)

            end

        end
